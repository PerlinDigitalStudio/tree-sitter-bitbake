# tree-sitter-bitbake

> [!NOTE]
> **This is a temporary fork of [tree-sitter-grammars/tree-sitter-bitbake](https://github.com/tree-sitter-grammars/tree-sitter-bitbake).**
> The `nacelle` branch is upstream master (a5d04fdb5a) with two open upstream pull requests:
>
> - [#24](https://github.com/tree-sitter-grammars/tree-sitter-bitbake/pull/24), "Update bindings & workflows": Rust bindings on `tree-sitter-language`. Zed, and Nacelle (our fork of Zed), build the grammar in with these. Upstream master still binds tree-sitter 0.20, which can't link next to a current tree-sitter.
> - [#23](https://github.com/tree-sitter-grammars/tree-sitter-bitbake/pull/23): `inherit_defer`, and variable expansions inside quoted strings in shell bodies, such as `echo "${D}/x"`. On a real Yocto tree, #23 gives about 8x fewer ERROR nodes on `.bb` files (454 against 3552).
>
> The files generated under `src/` come from `tree-sitter generate --abi 14` with tree-sitter CLI 0.25.6, the version #24 uses. Nothing else is changed. See [NOTICE](NOTICE) for the license and authors.
>
> This fork is archived when upstream merges both pull requests.

[![CI](https://github.com/amaanq/tree-sitter-bitbake/actions/workflows/ci.yml/badge.svg)](https://github.com/amaanq/tree-sitter-bitbake/actions/workflows/ci.yml)
[![Discord](https://img.shields.io/discord/1063097320771698699?logo=discord)](https://discord.gg/w7nTvsVJhm)

[BitBake](https://docs.yoctoproject.org/bitbake/) grammar for [tree-sitter](https://tree-sitter.github.io)
