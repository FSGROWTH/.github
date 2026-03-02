# CLAUDE.md

## Repository Overview

This is the `.github` organization-level repository for **FS Growth** (`FSGROWTH`). It houses the GitHub organization profile and shared configuration.

## Repository Structure

```mermaid
graph TD
    A["FSGROWTH/.github"] --> B["profile/"]
    B --> C["README.md<br/><i>Organization profile</i>"]

    style A fill:#1a1a2e,stroke:#e94560,color:#fff
    style B fill:#16213e,stroke:#0f3460,color:#fff
    style C fill:#0f3460,stroke:#533483,color:#fff
```

## Architecture Diagram

```mermaid
flowchart LR
    subgraph org["FSGROWTH GitHub Organization"]
        direction TB
        subgraph dotgithub[".github repo"]
            direction TB
            profile["profile/README.md"]
        end
    end

    visitor(["GitHub Visitor"]) -->|"visits github.com/FSGROWTH"| org
    org -->|"renders org profile from"| profile
    profile -->|"links to"| site(["fsgrowth.com"])

    style org fill:#1a1a2e,stroke:#e94560,color:#fff
    style dotgithub fill:#16213e,stroke:#0f3460,color:#fff
    style profile fill:#0f3460,stroke:#533483,color:#fff
    style visitor fill:#533483,stroke:#e94560,color:#fff
    style site fill:#533483,stroke:#e94560,color:#fff
```

## What This Repo Does

- **Organization Profile**: `profile/README.md` is rendered on the FSGROWTH GitHub organization page
- **Company**: FS Growth — non-dilutive equipment financing for high-growth tech and life sciences companies
- **Website**: [fsgrowth.com](https://www.fsgrowth.com)

## Development Notes

- This repo has no build steps, CI/CD, or dependencies
- Changes to `profile/README.md` are immediately reflected on the GitHub org page
- Keep the profile concise and on-brand
