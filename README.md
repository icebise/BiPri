<div align="center">
  <img src="BiPri.png" alt="BiPri Launcher Logo" width="150"/>
  <h1>BiPri Launcher</h1>
</div>

**Caution**

There are malicious links in the wild that may disguise themselves as this project. 

Make sure that you download BiPri Launcher only from the official sources: [icebise.github.io](https://icebise.github.io) and/or our GitHub Releases page.

This fork of Prism Launcher adds integrated support for Ely.by accounts (MSA accounts can still be used).

**This is not endorsed by Prism Launcher or Ely.by.**

## Why this fork?

Many forks add Ely.by support by simply adding a login-password prompt and authlib-injector download. BiPri Launcher goes beyond that:

*   **Modern and secure login:** BiPri uses OAuth2 to log you in. This means your credentials are never transferred to the launcher. Instead, you log into your account on the official Ely.by page in your browser, and Ely.by gives the launcher a token to access your account with limited privileges.
*   **Skins support on servers:** BiPri uses Ely.by's official Authlib patches, allowing you to see skins anywhere, even on servers that don't have special skins plugins installed.

## Installation

All downloads and instructions for BiPri Launcher can be found on the [Releases](https://github.com/icebise/BiPri/releases) page.

Last build status can be found in the GitHub Actions tab.

## Development Builds

Please understand that these builds are not intended for most users. There may be bugs, and other instabilities. You have been warned.

There are development builds available through:
*   GitHub Actions (includes builds from pull requests opened by contributors)
*   nightly.link (this will always point only to the latest version of develop)

These have debug information in the binaries, so their file sizes are relatively larger.

## Community & Support

Feel free to create a [GitHub issue](https://github.com/icebise/BiPri/issues) if you find a bug or want to suggest a new feature. 

Join our Discord server for community support and updates: [BiPri Launcher Discord](https://discord.gg/bhN7CaxNdc).

## Building

If you want to build BiPri Launcher yourself, check the build instructions.

## Forking/Redistributing/Custom builds policy

You are free to fork, redistribute and provide custom builds as long as you follow the terms of the license (this is a legal responsibility), and if you made code changes rather than just packaging a custom build, please do the following as a basic courtesy:

*   Make it clear that your fork is not Prism Launcher and is not endorsed by or affiliated with the Prism Launcher project (https://prismlauncher.org).
*   Go through `CMakeLists.txt` and change Prism Launcher's API keys to your own or set them to empty strings (`""`) to disable them.
*   If you have any questions, please refer to the original Prism Launcher guidelines.

Note that if you build this software without removing the provided API keys in `CMakeLists.txt` you are accepting the following terms and conditions:
*   Microsoft Identity Platform Terms of Use
*   CurseForge 3rd Party API Terms and Conditions

If you do not agree with these terms and conditions, then remove the associated API keys from the `CMakeLists.txt` file by setting them to an empty string (`""`).

## License

All launcher code is available under the **GPL-3.0-only** license.

The logo and related assets are under the **CC BY-SA 4.0** license.
