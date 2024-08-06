# exec

Provides a simple command for extensions to target to run shell commands.

## Features

Extensions can target this command from a UI host, such as a web extension, to run a task on the remote machine.

### Example

```typescript
await vscode.commands.executeCommand('exec.command', '/bin/bash -c "echo Hello, world!"');
await vscode.commands.executeCommand('exec.command', [
  '/bin/bash',
  '-c',
  'echo "Hello, world!"'
]);
```

## Extension Settings

This extension contributes the following commands:

- `exec.command`: Run a shell command on the remote machine.

## Known Issues

## Release Notes

### 0.0.1

Initial release!
