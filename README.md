<div align="center">

<img src="https://moebiusordernewsalternate.netlify.app/data/images/b2/banner.png" alt="MON CS DOCS Banner" width="800"/>

# MON CS DOCS Media CDN

### Official Asset Delivery Network for Computer Science Documentation

*High-Performance Visual Resources — Diagrams, Illustrations, and Educational Media*

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
[![CDN Status](https://img.shields.io/badge/CDN-Live-brightgreen)](https://media.moncsdocs.moebiusorder.com)
[![Managed by Moebius Order](https://img.shields.io/badge/Managed%20by-Moebius%20Order-blue)](https://www.moebiusorder.com)

**CDN Root**: [media.moncsdocs.moebiusorder.com](https://media.moncsdocs.moebiusorder.com)

[Main Docs Repo](https://github.com/Moebius-Order/moncsdocs) • [License](https://mcsdocs.moebiusorder.com/g/license) • [Community](https://t.me/moncsdocs) • [Donate](https://mcdocs.moebiusorder.com/donate)

</div>

---

## CDN & Repository Overview

**MonCSDocs Media CDN** is the centralized asset delivery network for the [MON CS DOCS](https://github.com/Moebius-Order/moncsdocs) documentation platform. This repository serves as the source-of-truth for all visual resources used across the web and mobile applications.

### Purpose

- **High-Performance Delivery**: Optimized asset serving via global CDN infrastructure
- **Centralized Management**: Single repository for all diagrams, illustrations, and graphics
- **Version Control**: Git-based tracking of all visual resource changes
- **Community Contributions**: Open submission process for educational diagrams
- **Legal Protection**: Clear licensing and copyright management for all assets

### CDN Root URL

All assets in this repository are accessible via:

```
https://media.moncsdocs.moebiusorder.com/<path-to-asset>
```

**Example**:
- Repository path: `/data/algorithms/binary-search-tree.svg`
- CDN URL: `https://media.moncsdocs.moebiusorder.com/data/algorithms/binary-search-tree.svg`

---

## Folder Architecture & Path Structure

### Directory Map

The repository is organized into three primary directories with distinct access levels:

```
moncsdocs-media/
├── logo/            [RESTRICTED] Official branding assets
│   ├── moebius-order-logo.png
│   ├── moncsdocs-logo.png
│   └── moncsdocs-banner.png
├── assets/          [RESTRICTED] Platform UI components
│   ├── icons/
│   ├── backgrounds/
│   └── ui-elements/
└── data/            [OPEN] Community-contributed educational assets
    ├── algorithms/
    ├── data-structures/
    ├── operating-systems/
    ├── networks/
    ├── databases/
    ├── computer-architecture/
    └── ...more topics
```

### `/logo` - Official Branding (RESTRICTED)

**Access Level**: Read-only for community contributors.

Contains official logos and brand assets:
- Moebius Order corporate logo
- MON CS DOCS project logo and banner
- Trademark-protected visual identity

> **Warning**: Pull Requests modifying this directory will be automatically rejected.

**Official Assets**:
- **MON CS DOCS Logo**: [https://moebiusordernewsalternate.netlify.app/data/images/b2/logo.png](https://moebiusordernewsalternate.netlify.app/data/images/b2/logo.png)
- **MON CS DOCS Banner**: [https://moebiusordernewsalternate.netlify.app/data/images/b2/banner.png](https://moebiusordernewsalternate.netlify.app/data/images/b2/banner.png)
- **Moebius Order Logo**: [https://moebiusorder.com/logo.png](https://moebiusorder.com/logo.png)

### `/assets` - Platform Components (RESTRICTED)

**Access Level**: Read-only for community contributors.

Contains proprietary UI elements used by the MON CS DOCS web and mobile applications:
- Interface icons and buttons
- Background patterns and textures
- Navigation graphics
- Application-specific visual components

> **Warning**: Pull Requests modifying this directory will be automatically rejected.

These assets are integral to the platform's proprietary design system and cannot be modified by external contributors.

### `/data` - Educational Content (OPEN FOR CONTRIBUTIONS)

**Access Level**: Open for community contributions.

> This is where **ALL community contributions must be placed**.

The `/data` directory contains:

- **Topic-Organized Diagrams**: Organized by CS subject area
- **Educational Illustrations**: Concept visualizations, flowcharts, state diagrams
- **Architectural Diagrams**: System designs, network topologies, hardware layouts
- **Algorithm Visualizations**: Step-by-step visual explanations
- **Data Structure Graphics**: Trees, graphs, heaps, hash tables

#### Subdirectory Organization

| Directory | Purpose | Examples |
|-----------|---------|----------|
| `/data/algorithms/` | Algorithm visualizations | `merge-sort.svg`, `dijkstra-shortest-path.png` |
| `/data/data-structures/` | Data structure diagrams | `red-black-tree.svg`, `hash-table-collision.png` |
| `/data/operating-systems/` | OS concepts | `process-lifecycle.svg`, `memory-paging.png` |
| `/data/networks/` | Networking diagrams | `tcp-handshake.svg`, `osi-model.png` |
| `/data/databases/` | Database concepts | `normalization-example.svg`, `b-tree-index.png` |
| `/data/computer-architecture/` | Hardware diagrams | `cpu-pipeline.svg`, `cache-hierarchy.png` |

### Path Logic: Repository to CDN Mapping

**How it works**:

1. You upload a file to the repository: `/data/algorithms/quicksort-partition.svg`
2. After merge, it becomes accessible via CDN: `https://media.moncsdocs.moebiusorder.com/data/algorithms/quicksort-partition.svg`
3. Documentation pages reference the CDN URL for fast, cached delivery

**Benefits**:
- Fast global delivery via CDN caching
- Automatic versioning through Git history
- Secure hosting with HTTPS
- Analytics and usage tracking

---

## Contribution Guidelines & Naming Conventions

### The "Data-First" Rule

> **CRITICAL**: All community contributions MUST be placed within the `/data/*` directory structure.

Contributions to `/logo` or `/assets` will be rejected without review.

### Naming Conventions for URL Optimization

To ensure clean, SEO-friendly, and accessible URLs, follow these strict naming rules:

#### 1. Lowercase Only

**Bad**: `BinarySearchTree.svg`, `TCP_Handshake.PNG`  
**Good**: `binary-search-tree.svg`, `tcp-handshake.png`

#### 2. Use Hyphens (-) Instead of Spaces or Underscores

**Bad**: `merge sort visualization.svg`, `heap_insertion.png`  
**Good**: `merge-sort-visualization.svg`, `heap-insertion.png`

#### 3. Descriptive and Specific Names

**Bad**: `diagram1.svg`, `image.png`, `fig-3.jpg`  
**Good**: `process-scheduling-round-robin.svg`, `b-plus-tree-insertion.png`

#### 4. Include Context in Name

Use the filename to describe what the asset represents:

- `quicksort-partition-step-1.svg`
- `osi-model-seven-layers.png`
- `cpu-cache-hierarchy-l1-l2-l3.svg`
- `tcp-three-way-handshake.png`

### File Format Standards

#### Preferred Formats (in order of priority)

**1. SVG (Scalable Vector Graphics)** — Best for diagrams, flowcharts, graphs
- Infinitely scalable
- Small file size
- Editable and accessible
- **Required** for: Algorithm flowcharts, data structure diagrams, system architecture

**2. WebP** — Best for complex illustrations with gradients/photos
- Superior compression
- Modern browser support
- Excellent quality-to-size ratio

**3. PNG** — Fallback for complex visuals
- Lossless compression
- Wide compatibility
- Use when SVG is not practical

#### Avoid These Formats

- **JPEG**: Lossy compression degrades diagram clarity
- **GIF**: Outdated, poor quality
- **BMP**: Uncompressed, massive file sizes

### Quality Standards

Before submitting, ensure your asset meets these criteria:

- **Clarity**: Text and labels are readable at typical screen resolutions
- **Simplicity**: Focused on explaining one concept clearly
- **Consistency**: Visual style matches existing assets (if applicable)
- **Optimization**: File size is minimized without quality loss
- **Accessibility**: Color choices work for colorblind users
- **Attribution**: Source information included if adapted from external work

### Contribution Workflow

```bash
# 1. Fork the repository
git clone https://github.com/YOUR-USERNAME/moncsdocs-media.git
cd moncsdocs-media

# 2. Create a topic branch
git checkout -b add/algorithms/quicksort-diagram

# 3. Add your asset to the appropriate /data subdirectory
mkdir -p data/algorithms
cp ~/my-diagram.svg data/algorithms/quicksort-partition.svg

# 4. Commit with descriptive message
git add data/algorithms/quicksort-partition.svg
git commit -m "Add: Quicksort partition step visualization"

# 5. Push and create Pull Request
git push origin add/algorithms/quicksort-diagram
```

### Pull Request Template

```markdown
### Asset Description
Quicksort partition step visualization showing pivot selection and array rearrangement.

### File Details
- Path: `/data/algorithms/quicksort-partition.svg`
- Format: SVG
- Size: 15 KB
- License: CC BY-SA 4.0

### Source & Attribution
- Original work created by [Your Name]
- Inspired by: [Reference if applicable]

### License Confirmation
I confirm that I own the copyright to this asset or have the legal right to contribute it under CC BY-SA 4.0.
```

---

## Permissions & Access Control

### Protected Paths

The following directories are **RESTRICTED** to Moebius Order maintainers only:

- `/logo/*` — Official branding and trademark assets
- `/assets/*` — Proprietary platform UI components

#### Automatic Rejection Policy

Any Pull Request that includes modifications to these directories will be:
1. Automatically flagged by CI/CD checks
2. Rejected without manual review
3. Closed with a standard explanation message

**Reasons for restriction**:

- **Brand Integrity**: Prevents unauthorized use or modification of trademarks
- **Platform Consistency**: Ensures UI components remain synchronized with application code
- **Legal Protection**: Maintains clear boundaries for intellectual property

### Permission Grant for `/data` Contributions

> **Important Understanding**: By uploading an asset to the `/data` directory, you grant Moebius Order specific rights.

**Rights granted**:

1. **CDN Distribution**: Right to serve your asset via `media.moncsdocs.moebiusorder.com`
2. **Format Conversion**: Right to optimize or convert formats for performance
3. **Caching**: Right to cache and replicate assets across CDN nodes globally
4. **Modification**: Right to resize, compress, or adapt assets for different devices/platforms
5. **Integration**: Right to embed assets in MON CS DOCS web and mobile applications

All rights are subject to **CC BY-SA 4.0 license** terms, meaning:
- Your attribution will be preserved
- Derivatives must maintain the same license
- Commercial use is permitted

---

## Legal & Liability Protection

### Host Disclaimer

**CRITICAL LEGAL NOTICE**:

> **Moebius Order acts as a SERVICE PROVIDER and HOSTING PLATFORM** for community-contributed media assets in the `/data` directory.

**Moebius Order is NOT**:
- The original author or copyright holder of community-submitted assets
- Responsible for verifying copyright ownership before publication
- Liable for copyright infringement claims arising from user contributions
- An endorser or guarantor of asset accuracy or quality

**Moebius Order operates under**:
- Digital Millennium Copyright Act (DMCA) safe harbor provisions (U.S.)
- E-Commerce Directive Article 14 hosting exemption (EU)
- Similar international intermediary liability protections

### Contributor Warranty

By contributing to `/data`, you represent and warrant:

1. You are the original creator, OR you have obtained all necessary rights
2. Your contribution does not infringe any third-party intellectual property
3. You have the legal authority to license the asset under CC BY-SA 4.0
4. You will indemnify Moebius Order against claims arising from your contribution

See [LICENSE](LICENSE) for full contributor warranty terms.

### DMCA Takedown Protocol

**For Copyright Holders**:

If you believe an asset in this repository infringes your copyright, submit a takedown notice.

#### Required Information

1. Your contact details (name, address, email, phone)
2. Identification of your copyrighted work
3. Specific file path (e.g., `/data/algorithms/example.svg`) and CDN URL
4. Good faith statement that use is unauthorized
5. Statement under penalty of perjury that information is accurate
6. Physical or electronic signature

#### Submit To

- **Email**: [moncsdocs@moebiusorder.com](mailto:moncsdocs@moebiusorder.com)
- **Subject**: "DMCA Takedown Notice - moncsdocs-media"

#### Response Timeline

Moebius Order will respond within **48-72 hours** and will:
1. Remove or disable access to the allegedly infringing material
2. Notify the contributor who uploaded the content
3. Provide counter-notice instructions if applicable

### Counter-Notice Procedure

If your content was removed and you believe it was a mistake:

1. Submit a counter-notice explaining why the content is not infringing
2. Include your contact information and signature
3. Consent to jurisdiction of federal court (or local equivalent)
4. Accept service of process from the original claimant

After 10-14 business days (unless the claimant files a lawsuit), content may be restored.

---

## Funding & CDN Infrastructure

**MON CS DOCS Media CDN is provided free of charge** to support open education.

### Infrastructure Costs

Maintaining a high-performance CDN requires ongoing investment:

| Component | Description |
|-----------|-------------|
| **CDN Bandwidth** | Global content delivery and edge caching |
| **Storage** | Scalable object storage for thousands of assets |
| **Security** | SSL certificates, DDoS protection, access control |
| **Optimization** | Automatic image compression and format conversion |
| **Monitoring** | Uptime tracking, performance analytics, error logging |
| **Maintenance** | Server management, updates, backups |

### Support the CDN

Help us keep the media infrastructure fast, secure, and ad-free.

Click the **Sponsor** button at the top of this repository, or visit:

- **Website**: [mcdocs.moebiusorder.com/donate](https://mcdocs.moebiusorder.com/donate)
- **Patreon**: [patreon.com/moebius_order](https://patreon.com/moebius_order)
- **Ko-fi**: [ko-fi.com/moebiusorder](https://ko-fi.com/moebiusorder)
- **Buy Me a Coffee**: [buymeacoffee.com/moebiusorder](https://buymeacoffee.com/moebiusorder)

Every contribution helps us:
- Increase CDN bandwidth capacity
- Improve global delivery speeds
- Expand storage for more assets
- Enhance security and reliability

---

## Community & Support

Join the MON CS DOCS community:

- **Telegram Channel**: [t.me/moncsdocs](https://t.me/moncsdocs) — Updates and announcements
- **Telegram Chat**: [t.me/moncsdocschat](https://t.me/moncsdocschat) — Questions and discussions
- **Discord**: [discord.gg/yb6XgkhBXU](https://discord.gg/yb6XgkhBXU) — Real-time collaboration
- **Reddit**: [r/moncsdocs](https://www.reddit.com/r/moncsdocs) — Long-form discussions

### Contact

- **Email**: [moncsdocs@moebiusorder.com](mailto:moncsdocs@moebiusorder.com)
- **Organization**: [Moebius Order](https://www.moebiusorder.com)

---

## License & Copyright

### Asset License

<div align="center">

[![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/)

</div>

All assets in the `/data` directory are licensed under the **[Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/)**.

**You are free to**:
- Share — Copy and redistribute assets
- Adapt — Remix, transform, and build upon assets
- Commercial use — Use in commercial projects

**Under these terms**:
- **Attribution** — Credit "MonCSDocs Media by Moebius Order and contributors"
- **ShareAlike** — Derivatives must use the same license

### Trademark Notice

> **Assets in `/logo` and `/assets` are NOT covered by CC BY-SA 4.0.**

The following are registered trademarks of **Moebius Order**:
- "Moebius Order" name and logo
- "MON CS DOCS" name and logo
- Visual brand identity and design system

Unauthorized use of trademarks is prohibited. Contact [moncsdocs@moebiusorder.com](mailto:moncsdocs@moebiusorder.com) for licensing inquiries.

### Copyright Statement

© 2026 **Moebius Order**. Community-contributed assets in `/data` licensed under CC BY-SA 4.0. Trademarks and proprietary assets remain exclusive property of Moebius Order.

For complete license terms, see [LICENSE](LICENSE) or visit [mcsdocs.moebiusorder.com/g/license](https://mcsdocs.moebiusorder.com/g/license).

---

## Quick Links

- **Main Documentation**: [github.com/Moebius-Order/moncsdocs](https://github.com/Moebius-Order/moncsdocs)
- **Website**: [mcdocs.moebiusorder.com](https://mcdocs.moebiusorder.com)
- **CDN**: [media.moncsdocs.moebiusorder.com](https://media.moncsdocs.moebiusorder.com)
- **License**: [mcsdocs.moebiusorder.com/g/license](https://mcsdocs.moebiusorder.com/g/license)
- **Community**: [t.me/moncsdocs](https://t.me/moncsdocs)
- **Donate**: [mcdocs.moebiusorder.com/donate](https://mcdocs.moebiusorder.com/donate)

---

<div align="center">

**Powering Visual Education for Computer Science**

Managed by [Moebius Order](https://www.moebiusorder.com) | Assets licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

<img src="https://moebiusordernewsalternate.netlify.app/data/images/b2/logo.png" alt="MON CS DOCS" width="100"/>

</div>