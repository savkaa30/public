# Privacy Policy — Andrej 3.0

Effective date: 8 November 2026

## Scope and contact
Andrej 3.0 (Oura application display name: Andrej3_0) is a personal integration being configured to retrieve the owner's Oura data for personal tracking and analysis. It is not currently offered as a public service. The operator and contact is Andrej Savka, savka.a@gmail.com.

The integration is configured for daily collection after the owner completes authorization. This policy describes that configuration and must be updated before other users are admitted or material data handling changes are introduced.

## Data and purpose
After the owner authorizes access through Oura, the integration is intended to retrieve daily sleep, activity and readiness summaries for personal reports and comparisons over time. Other categories, such as heart rate, workouts, tags, sessions, oxygen saturation, stress or heart health, may be retrieved only if enabled and authorized for a feature the owner chooses to use. Email, profile and ring configuration access should be left disabled unless needed.

## Authorization and control
Oura credentials are entered with Oura through its authorization flow, not collected by this application. OAuth access and refresh tokens enable the authorized connection and must be treated as secrets. The owner can revoke the integration's access through Oura. Revocation stops future authorized retrieval; it does not automatically delete previously exported copies.

## Storage and retention
Oura records are stored in the owner's private GitHub repository, savkaa30/andrej3_0, and processed by GitHub Actions for scheduled retrieval. Exported health records are not additionally encrypted by this integration; repository access controls protect access. OAuth tokens are stored there as authenticated ciphertext, encrypted using a key derived from the Oura Client Secret. The Client Secret is stored separately in GitHub Actions secrets. A short-lived authorization code and PKCE verifier are temporarily stored on the owner's computer and in an Actions secret during initial setup and should be deleted after successful setup. No health records or credentials are published in this public documentation repository.\n\nArchives are retained until the owner deletes them. Record updates replace the current version but previous versions may remain in Git history and service backups. Removing a file in a new commit does not erase prior commits. Revocation and deletion must therefore include any relevant repository history and backups, subject to GitHub's retention controls.

## AI analysis and third parties
AI analysis is optional. If the owner enables an OpenAI or other AI integration, selected Oura data and related prompts will be sent to that provider to generate the requested analysis. Its own terms, privacy settings and retention rules will apply. This policy does not claim that such transmission has already been enabled. The configured GitHub Actions workflow only downloads and archives Oura data; it does not send health data to an AI provider. GitHub supplies repository hosting and automation, subject to its own terms and privacy practices.

The integration is intended solely for the owner's personal use, with no sale of Oura data, advertising use or public publication of health records.

## Access, deletion and questions
The owner can stop collection, revoke access and delete copies under their control. For questions or assistance with access or deletion, contact savka.a@gmail.com. Deletion from Oura or third-party services must be handled using those services' controls.

## Changes
The effective date will be updated when this policy changes. Before broader use or material changes in data handling, this policy must be revised to reflect the actual implementation.
