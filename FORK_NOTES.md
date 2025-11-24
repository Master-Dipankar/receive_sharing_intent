# Fork Notes

## Why This Fork Exists

This fork of `receive_sharing_intent` was created to address a critical JVM-target compatibility issue that was causing build failures in downstream projects.

### Fixed Issue

**JVM-target compatibility** (Commit: `2cea396843cd3ab1b5ec4334be4233864637874e`)
- Fixed inconsistent JVM-target compatibility between different modules
- Ensures proper compilation with modern Kotlin and Java versions
- Reference: [PR #333](https://github.com/KasemJaffer/receive_sharing_intent/pull/333)

## How to Use This Fork

### Pin to a Tag (Recommended)

Add this to your `pubspec.yaml`:

```yaml
dependencies:
  receive_sharing_intent:
    git:
      url: https://github.com/Master-Dipankar/receive_sharing_intent.git
      ref: v1.8.1-fixed
```

### Pin to a Commit

Alternatively, pin to the exact commit hash:

```yaml
dependencies:
  receive_sharing_intent:
    git:
      url: https://github.com/Master-Dipankar/receive_sharing_intent.git
      ref: 2cea396843cd3ab1b5ec4334be4233864637874e
```

## Safety Recommendations

### Best Practices

1. **Prefer Tags Over Branches**: Tags are immutable and provide clear versioning
2. **Use Dependabot**: Set up automated checks for upstream changes
3. **License Compliance**: This project uses Apache License 2.0 - ensure proper attribution
4. **Keep a Changelog**: Document all fork-specific changes
5. **Test Before Merging**: Always run CI/CD before adopting upstream changes

### Monitoring Upstream

- **Upstream Repository**: [KasemJaffer/receive_sharing_intent](https://github.com/KasemJaffer/receive_sharing_intent)
- **Watch for Updates**: Monitor for new releases and security patches
- **Selective Merging**: Cherry-pick specific fixes rather than blindly merging all changes

## When to Merge Upstream

1. **After Testing**: Only merge after confirming compatibility with your project
2. **Security Patches**: Prioritize security-related updates
3. **Bug Fixes**: Evaluate each bug fix for relevance to your use case
4. **Feature Updates**: Consider whether new features are needed before merging

## Fork Changelog

### v1.8.1-fixed (2024)
- Fixed JVM-target compatibility issue
- Ensures consistent build configuration across Kotlin modules
- Based on upstream commit 2cea396

## Contributing

If you find issues specific to this fork or want to contribute improvements:
1. Open an issue in this repository
2. Submit a pull request with clear description
3. Ensure all tests pass before requesting review

## Upstream Synchronization

Last synchronized with upstream: Check git log for latest merge commits
Next scheduled review: Monitor upstream releases regularly

## License

This fork maintains the original Apache License 2.0.
See [LICENSE](LICENSE) for full terms.
