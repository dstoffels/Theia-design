# Theia Design Subtree
This subtree contains game design documents and resources, tracked in the [game design repository](https://github.com/dstoffels/Theia-design.git) to keep design work isolated from the codebase.

When working in the [Theia-design](https://github.com/dstoffels/Theia-design.git) repository, always pull the latest changes before referencing these docs in development:
```bash
git subtree pull --prefix=design https://github.com/dstoffels/Theia-design.git main --squash
```

If edits or corrections are made in the [main game repository](https://github.com/dstoffels/Theia.git), they must be pushed back to the [Theia-design](https://github.com/dstoffels/Theia-design.git) repository:
```bash
git subtree push --prefix=design https://github.com/dstoffels/Theia-design.git main
```