# Repository workflow

After completing a user-requested change and performing proportionate verification, automatically:

1. Stage only files directly related to the completed task (do not stage unrelated pre-existing changes).
2. Create a concise commit that describes the change.
3. Push the current branch to `origin`.

Do not wait for a separate request to commit or push. Do not commit or push when the user explicitly asks not to, or when verification identifies an unresolved failure that would make the change unsafe to publish. Report the commit hash and push result in the final response.
