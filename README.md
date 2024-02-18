# Qualcommax_NSS_Builder

This project automates OpenWRT builds for the Xiaomi AX3600, focusing on comprehensive NSS support with a minimalistic approach to additional packages. It is based on the `qualcommax-6.1-nss-wifi` branch from [qosmio/openwrt-ipq](https://github.com/qosmio/openwrt-ipq/tree/qualcommax-6.1-nss-wifi) and draws inspiration from [rodriguezst/ipq807x-openwrt-builder](https://github.com/rodriguezst/ipq807x-openwrt-builder).

## Features

The build features:
- **Full NSS (Network Subsystem) support** for enhanced networking performance, including:
  - Essential NSS configurations
  - NSS drivers for PPPoE, Qdisc, and IFB: `CONFIG_PACKAGE_kmod-qca-nss-drv-pppoe=y`, `CONFIG_PACKAGE_kmod-qca-nss-drv-qdisc=y`, `CONFIG_PACKAGE_kmod-nss-ifb=y`
- **LuCI**, a web-based GUI for OpenWRT, for easy system administration.
- **SQM (Smart Queue Management)** support to reduce bufferbloat, enhance overall network responsiveness, and manage network traffic effectively. Includes `luci-app-sqm` and `sqm-scripts-nss`. For configuration details, refer to [SQM Scripts NSS documentation](https://github.com/rickkdotnet/sqm-scripts-nss).
- **Security and Network Management Tools**:
  - `luci-app-banip` for IP-based banning.
  - `luci-ssl` to secure the LuCI web interface with SSL/TLS.
- **Comprehensive Wireless Protocol Support** with `wpad-mbedtls` (Full).

## Contributing

Contributions are highly appreciated! If you have suggestions for additional packages, essential features that are missing, or improvements to the existing setup, please feel free to submit a pull request or open an issue. Your input helps make Qualcommax_NSS_Builder even better for everyone.