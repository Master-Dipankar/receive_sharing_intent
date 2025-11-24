# Tag Push Instructions

## Repository Maintainer Note

A git tag `v1.8.1-fixed` has been created locally and needs to be pushed to the remote repository.

### To Push the Tag

Run the following command from the repository root:

```bash
git push origin v1.8.1-fixed
```

### Tag Details

- **Tag Name**: `v1.8.1-fixed`
- **Purpose**: Marks the fork release with JVM-target compatibility fixes
- **Commit**: Points to the commit with fork documentation
- **Base Fix**: Built on commit `2cea396843cd3ab1b5ec4334be4233864637874e`

### After Pushing

Once the tag is pushed, users can reference it in their `pubspec.yaml`:

```yaml
dependencies:
  receive_sharing_intent:
    git:
      url: https://github.com/Master-Dipankar/receive_sharing_intent.git
      ref: v1.8.1-fixed
```

### Verification

To verify the tag was pushed successfully:

```bash
git ls-remote --tags origin
```

Look for `refs/tags/v1.8.1-fixed` in the output.

### Creating a GitHub Release (Optional)

For better visibility, you can also create a GitHub Release:

1. Navigate to your repository on GitHub and go to the Releases page (`/releases/new` path)
2. Choose the tag: `v1.8.1-fixed`
3. Title: "v1.8.1-fixed - JVM-target Compatibility Fix"
4. Description: Use content from FORK_NOTES.md
5. Publish the release

This makes it easier for users to discover and use the fork.
