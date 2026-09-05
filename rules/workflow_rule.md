# Workflow Rule

## Discussion Mode

When the user is discussing ideas, copy, layout, structure, or a modification plan in ChatGPT mode, do not modify project files.

Use this mode for:

- planning changes
- discussing content
- rewriting text
- comparing layout ideas
- deciding what the final result should be

The user may say:

```text
Discuss only, don't modify files.
```

or:

```text
先不要改檔案，只討論修改方案。
```

## Codex Execution Mode

Only modify code, HTML, CSS, assets, git commits, or GitHub pushes after the user confirms the result and explicitly asks Codex to execute the change.

The user may say:

```text
This is final. Please let Codex update the project files.
```

or:

```text
Now modify the HTML and push to GitHub.
```

or:

```text
現在請直接修改 HTML，然後 commit/push。
```

## Default Rule

If the user is still discussing or reviewing a proposed result, stay in discussion mode.

If the user clearly asks for implementation, Codex should:

1. read the relevant project files
2. make the requested modifications
3. verify links, paths, and visible references
4. commit the change when appropriate
5. push to GitHub when explicitly requested
