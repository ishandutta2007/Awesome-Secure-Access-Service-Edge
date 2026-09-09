# Awesome-Secure-Access-Service-Edge

## Top Secure Access Service Edge (SASE) Platforms Ecosystem
**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Converged Networking + Security, ZTNA, SSE, SD-WAN, Cloud SWG, CASB & Zero Trust Access*
**Last updated: September 2026**

This repository tracks notable **SaaS / cloud platforms** and **open-source projects** for **Secure Access Service Edge (SASE)**. SASE converges SD-WAN-style networking with cloud-delivered security services (ZTNA, SWG, CASB, FWaaS, DLP) so users and sites connect securely to apps and the internet without traditional VPNs or appliance stacks.

**Examples** include Cloudflare One, Zscaler, Netskope, Cato Networks, Palo Alto Prisma SASE, Cisco Secure Access, Versa SASE, Fortinet FortiSASE, Check Point Harmony SASE, and Open Systems (the category leaders).

**Open-source emphasis**: A complete multi-PoP commercial SASE fabric (global inspection points, full SWG/CASB/DLP) remains largely proprietary. Strong open-source building blocks exist for the **Zero Trust / mesh / ZTNA** layer — **NetBird**, **Headscale**, **WireGuard**, **OpenZiti**, **Nebula**, and related projects. This section lists those options and is realistic about the remaining gap for full SSE.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms
- **[Cloudflare One](https://www.cloudflare.com/cloudflare-one/)**  
  SASE / Zero Trust platform built on Cloudflare’s global edge — Access (ZTNA), Gateway (SWG), WARP, and related services with strong developer and performance focus.

- **[Zscaler](https://www.zscaler.com/)**  
  Pioneer cloud security platform (ZIA / ZPA / ZDX) delivering large-scale SSE, zero-trust access, and internet/private-app security without backhauling to a data center.

- **[Netskope](https://www.netskope.com/)**  
  Intelligent SSE platform especially strong in CASB, data protection/DLP, and visibility into SaaS and cloud activity.

- **[Cato Networks](https://www.catonetworks.com/)**  
  Single-vendor SASE with private global backbone, converged networking and security, and operational simplicity.

- **[Palo Alto Prisma SASE](https://www.paloaltonetworks.com/sase)**  
  Prisma Access and related SASE offerings bringing NGFW-grade inspection, threat prevention, and ZTNA into a cloud-delivered model.

- **[Cisco Secure Access](https://www.cisco.com/)**  
  Cisco’s SASE / secure access portfolio (including Umbrella heritage) for organizations standardized on Cisco networking and security.

- **[Versa SASE](https://versa-networks.com/)**  
  Multi-tenant SASE platform combining SD-WAN, security, and cloud services with strong price/performance positioning.

- **[Fortinet FortiSASE](https://www.fortinet.com/)**  
  Cloud-delivered SASE integrated with the Fortinet Security Fabric and FortiOS policy model.

- **[Check Point Harmony SASE](https://www.checkpoint.com/)**  
  Harmony SASE (and related Zero Trust / remote access offerings) focused on prevention-first cloud security.

- **[Open Systems](https://www.open-systems.com/)**  
  Managed SASE and secure networking services oriented toward operational simplicity and global connectivity.

## Open-Source GitHub Projects
- **[NetBird](https://github.com/netbirdio/netbird)**  
  Fully self-hostable WireGuard-based mesh VPN and Zero Trust platform with management UI, SSO/MFA, granular ACLs, posture checks, and relays — one of the strongest open ZTNA/mesh alternatives.

- **[Headscale](https://github.com/juanfont/headscale)**  
  Open-source, self-hosted implementation of the Tailscale control server — use official Tailscale clients against your own coordination plane.

- **[WireGuard](https://www.wireguard.com/)**  
  Modern, high-performance VPN protocol and kernel implementation that underpins most open mesh/ZTNA solutions.

- **[OpenZiti](https://github.com/openziti)**  
  Open-source zero-trust networking platform with identity-based, application-embedded overlays and “dark” services (no open ports).

- **[Nebula](https://github.com/slackhq/nebula)**  
  Scalable overlay networking tool from Slack — lightweight, certificate-based mesh suitable for large distributed environments.

- **[ZeroTier](https://github.com/zerotier)**  
  Virtual Ethernet / mesh networking (open components with commercial control plane options) for easy multi-site connectivity.

- **[pfSense / OPNsense](https://www.pfsense.org/)**  
  Open-source firewall and routing platforms frequently used as SD-WAN or secure edge building blocks at sites.

- **[Tailscale clients + open control options](https://tailscale.com/)**  
  Clients are usable with Headscale; the broader ecosystem demonstrates the mesh + identity model that commercial SASE builds upon.

- **[Open-source SWG / proxy and filtering stacks](https://github.com/)**  
  Squid, e2guardian, and related tools that can approximate basic secure web gateway functions when combined with identity and policy.

- **[Identity-aware proxy and tunnel projects](https://github.com/)**  
  Various open reverse-proxy and tunnel solutions (including Cloudflare Tunnel open components and alternatives) used for application-level Zero Trust access.

### Additional Strong Open-Source Options
- Deploying **NetBird** or **Headscale + Tailscale clients** as a self-hosted ZTNA / mesh replacement for traditional VPNs.
- Using **OpenZiti** when application-embedded, portless zero-trust connectivity is preferred over device mesh.
- Combining **WireGuard** or **Nebula** with your own identity provider (Keycloak, Authentik, etc.) and policy scripts.
- Running **OPNsense/pfSense** at branches for local security and SD-WAN-like routing into a central open mesh.
- Accepting that full cloud SWG, CASB, advanced DLP, and global inspection PoPs still require commercial SASE/SSE platforms.
- Hybrid approaches: open ZTNA for private apps + commercial SSE for internet/SaaS traffic.

**Frameworks for building custom systems**: Build Zero Trust access with **NetBird** or **Headscale**, encrypt traffic with **WireGuard**, enforce identity via open IdPs, and optionally front apps with open identity-aware proxies. Add open firewalls at sites. This covers a large portion of the “secure remote access” problem. Commercial SASE (Cloudflare One, Zscaler, Netskope, Cato, Prisma, etc.) remains the practical choice when you need global PoPs, full SSE (SWG/CASB/DLP/FWaaS), unified policy, and vendor-operated scale.

## How to Contribute
1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer
- This is a **community-curated** list — not exhaustive and not an endorsement.
- SASE and Zero Trust deployments affect how every user and site reaches applications and the internet. Misconfiguration can lock out users or expose resources. Open-source components require careful hardening, monitoring, key management, and operational ownership. Always test failover, posture checks, and policy changes in non-production environments first. Compliance (data residency, logging, etc.) remains the organization’s responsibility.
- This list is not security or network architecture advice.

---
**Made for security architects, network engineers, and platform teams building least-privilege access without legacy VPN pain.**
Let's keep connectivity encrypted, identity-aware, and as open as the threat model allows.
