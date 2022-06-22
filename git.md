# Git commit standard
(type)[(optional scope)](optional breaking change): (subject) 

(optional body) 

(optional footer) 

## Header
### Type
**chore**: Changes that affect the build system or external dependencies

**ci**: Changes to the CI configuration

**docs**: Documentation only changes

**feat**: New feature

**fix**: Bug fix

**perf**: Code change that improves performance

**refactor**: Code change that neither fixes a bug nor adds a new feature

**revert**: Reverts commit (If the commit reverts a previous commit, it should begin with revert: , followed by the header of the reverted commit. In the body it should say: This reverts commit "hash", where the hash is the SHA of the commit being reverted.)

**style**: Does not affect meaning of the code (formatting)
test: Add or corrects tests

### Scope
A scope MAY be provided after a type. A scope MUST consist of a noun describing a section of the codebase surrounded by parenthesis, e.g., fix(parser):
### Breaking change
BREAKING CHANGE: a commit that has a footer BREAKING CHANGE:, or appends a ! after the type/scope, introduces a breaking API change (correlating with MAJOR in Semantic Versioning). A BREAKING CHANGE can be part of commits of any type.
### Subject
use the imperative, present tense: "change" not "changed" nor "changes"

don't capitalize the first letter

no dot (.) at the end

maximum 50 letters
## Body
Just as in the subject, use the imperative, present tense: "change" not "changed" nor "changes". The body should include the motivation for the change and contrast this with previous behavior.

maximum 72 letters per line
## Footer
The footer should contain any information about Breaking Changes and is also the place to reference GitHub issues that this commit Closes.

Example:

Resolves: #123

See also: #456

Reverts: #789

Breaking Changes should start with the word BREAKING CHANGE: with a space or two newlines. The rest of the commit message is then used for this.
