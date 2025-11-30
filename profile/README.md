# Migration Script Runner

Database-agnostic migration framework for TypeScript and JavaScript.

## What makes it different

**Works with any database** — SQL, NoSQL, or custom. You control the database operations, MSR handles the migration workflow.

**Library-first design** — Returns structured results instead of calling `process.exit()`. Safe for production apps, web servers, and serverless functions.

**Flexible rollback** — Choose your strategy: automatic backup/restore, down() methods, both, or none.

## Quick example

```typescript
const executor = new MigrationScriptExecutor(handler, config);
const result = await executor.up();

if (result.success) {
  console.log(`Executed ${result.executed.length} migrations`);
}
```
  
 ## Get started

- 📖 [Documentation](https://migration-script-runner.github.io/msr-core/)
- 🚀 [Quick Start](https://migration-script-runner.github.io/msr-core/getting-started)
- 💬 [Discussions](https://github.com/migration-script-runner/msr-core/discussions)

---

Photo by [Logan Voss](https://unsplash.com/@loganvoss?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/photos/abstract-streaks-of-pink-and-blue-neon-lights-xOFg66ATMnc?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
