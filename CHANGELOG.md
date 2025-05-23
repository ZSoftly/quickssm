# Changelog

All notable changes to the ZTiAWS project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [v1.4.2] - 2025-05-10

### Added
- Remote command execution capabilities
  - New `exec` command to run commands on individual EC2 instances
  - New `exec-tagged` command to run commands across multiple instances with the same tag
  - Real-time status updates during command execution
  - Formatted output display showing both stdout and stderr
- Enhanced error handling for missing instances and command failures

### Fixed
- Improved AWS SSO token management with better cache file detection
- Fixed "base64: invalid input" errors when using exec-tagged command
- Resolved ShellCheck warnings for improved CI pipeline reliability

## [v1.4.1] - 2025-05-10

### Added
- Enhanced error handling for access token retrieval in authaws script

### Fixed
- Improved error messages for SSO configuration issues

## [v1.4.0] - 2025-03-30

### Added
- Renamed auth script from auth_aws to authaws for better usability
- Ensured PATH updates with proper commenting and new line handling

## [v1.3.1] - 2025-03-31

### Changed
- Rebranded repository to ZTiAWS from quickssm
- Updated documentation, README, and issue templates to reflect new branding
- Improved installation and troubleshooting guides

## [v1.3.0] - 2025-05-10

### Added
- Support for running commands on EC2 instances (initially named run_command)
- Improved tests for the SSM script

### Fixed
- Syntax error in detect_os function
- ShellCheck directive placement in cleanup function

## [v1.1.2] - 2025-03-28

### Added
- New auth_aws script for simplified AWS SSO login
- Improved logging functionality
- Better error handling

## [v1.1.0] - 2025-02-06

### Added
- Support for Singapore region (ap-southeast-1)
- Formatted EC2 instance output with clear columns
- PowerShell profile for Windows users

## [v1.0.0] - 2025-01-20 (Initial Release)

### Added
- Core SSM Session Manager functionality
- Support for multiple regions
- Auto-install prompt for AWS SSM plugin
- Basic documentation and README
- Installation support for bash and zsh
- Initial CI/CD setup with badges