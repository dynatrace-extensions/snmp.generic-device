# Generic Device

This extension leverages the SNMP protocol to provide a complete solution to monitor network infrastructure. The complete configuration is provided out-of-the-box.

**This is intended for users, who:**

- Would like to monitor health state and performance of their core network infrastructure and provide unified analysis for Ops, DevOps and IT Admins.

**This enables you to:**

- Monitor health and performance of your network devices
- Set up alerts to be notified by traffic anomalies

**Compatibility Requirements**

- standard network devices supporting common MIB files
- SNMPv2c and SNMPv3 supported only

## Dev

### Prerequisites
- Nix-capable environment, for Windows that means [installing WSL](https://docs.microsoft.com/en-us/learn/modules/get-started-with-windows-subsystem-for-linux/2-enable-and-install)
- [nix](https://nixos.org/download.html) / [**nix for WSL**](https://nixos.org/download.html#nix-install-windows)
- `direnv` (`nix-env -iA nixpkgs.direnv`)
- [configured direnv shell hook ](https://direnv.net/docs/hook.html), yup in your `.bashrc`
- some form of `make` (`nix-env -iA nixpkgs.gnumake`)
- Docker (available in the same environment as nix)

Hint: if something doesn't work because of missing package please add the package to `default.nix` instead of installing on your computer. Why solve the problem for one if you can solve the problem for all? ;)

### One-time setup
```
make init
```

### Everything
```
make help
```

### Resources
- [Extension yaml docs](https://www.dynatrace.com/support/help/extend-dynatrace/extensions20/extension-yaml)
- [Extension knowledge base](https://www.dynatrace.com/support/help/extend-dynatrace/extensions20)

### Internal tooling
If you're a **Dynatrace employee** you can follow [this link](https://github.com/dynatrace-extensions/precious-toolz-internal) to enable internal tooling






