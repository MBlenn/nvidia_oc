# nvidia_oc

These are the real repositories for nvidia_oc, you should try and obtain an up-to-date release from first:
https://github.com/Dreaming-Codes/nvidia_oc
https://crates.io/crates/nvidia_oc

However, the official release wouldn't work on one systems, so I'm sharing the recompiled (now working) executable here.

2025.02.25 - 0.1.18:
The current official nvidia_oc release wouldn't work on Ubuntu 22.04 since it was compiled on a newer glibC.
Cargo wouldn't compile it on Ubuntu 22.04 due to an outdated rust compiler ("home" needed rustc-1.81 but only rustc-1.80 is available in 22.04)
Downgrade of module "home" to 0.5.9 fixed it and allowed the compile with rustc-1.80.
