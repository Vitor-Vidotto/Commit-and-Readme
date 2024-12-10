# Commit Standards 📜

According to the **[Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)** documentation, semantic commits are a simple convention to be used in commit messages. This convention defines a set of rules for creating an explicit commit history, which facilitates the creation of automated tools.

These commits will help you and your team to easily understand which changes were made in the chunk of code that was committed.

This identification occurs through a word and emoji that indicate whether the commit is related to a code change, package update, documentation, UI change, test, and more.

## Type and Description 🦄

A semantic commit has the following structural elements (types), which inform the user of your code about the intent of your commit:

- `feat` - Commits of this type indicate that your code section includes a **new feature** (related to the MINOR version of semantic versioning).
  
- `fix` - Commits of this type indicate that your code section is **fixing a problem** (bug fix), (related to the PATCH version of semantic versioning).
  
- `docs` - Commits of this type indicate **documentation changes**, such as changes to your repository's README (does not include code changes).
  
- `test` - Commits of this type are used when there are **changes to tests**, such as creating, modifying, or deleting unit tests (does not include code changes).
  
- `build` - Commits of this type are used when there are changes to **build files and dependencies**.
  
- `perf` - Commits of this type identify any code changes related to **performance**.
  
- `style` - Commits of this type indicate changes related to **code formatting**, semicolons, trailing spaces, linting, etc. (does not include code changes).
  
- `refactor` - Commits of this type refer to changes due to **refactoring that does not alter functionality**, such as changing how a part of the screen is processed but maintaining the same functionality, or improving performance due to a code review.
  
- `chore` - Commits of this type indicate **updates to tasks** like build, admin configurations, packages, etc., such as adding a package to `.gitignore` (does not include code changes).
  
- `ci` - Commits of this type indicate changes related to **continuous integration**.
  
- `raw` - Commits of this type indicate changes related to configuration files, data, features, or parameters.
  
- `cleanup` - Commits of this type are used to remove commented-out code, unnecessary sections, or any other kind of codebase cleanup aimed at improving readability and maintainability.
  
- `remove` - Commits of this type indicate the deletion of obsolete or unused files, directories, or features, reducing the size and complexity of the project and keeping it more organized.

## Recommendations 🎉

- Add a type consistent with the content's title.
- We recommend keeping the first line to a maximum of 4 words.
- To describe in detail, use the commit description.
- Use an emoji at the beginning of the commit message that represents the commit.
- Links should be added in their most authentic form, i.e., no URL shorteners or affiliate links.

## Commit Complements 💻

- **Footer:** Information about the reviewer and the card number on Trello or Jira. Example: Reviewed-by: Elisandro Mello Refs #133.
- **Body:** More detailed descriptions of what is contained in the commit, its impacts, and the reasons behind the changes made to the code, as well as essential instructions for future interventions. Example: See the issue for details on typos fixed.
- **Descriptions:** A brief description of the change. Example: Correct minor typos in code.

## Emoji Standards 💈

<table>
  <thead>
    <tr>
      <th>Commit Type</th>
      <th>Emoji</th>
      <th>Keyword</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Accessibility</td>
      <td>♿ <code>:wheelchair:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Adding a test</td>
      <td>✅ <code>:white_check_mark:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Updating a submodule version</td>
      <td>⬆️ <code>:arrow_up:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Rolling back a submodule version</td>
      <td>⬇️ <code>:arrow_down:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Adding a dependency</td>
      <td>➕ <code>:heavy_plus_sign:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Code review changes</td>
      <td>👌 <code>:ok_hand:</code></td>
      <td><code>style</code></td>
    </tr>
    <tr>
      <td>Animations and transitions</td>
      <td>💫 <code>:dizzy:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Bug fix</td>
      <td>🐛 <code>:bug:</code></td>
      <td><code>fix</code></td>
    </tr>
    <tr>
      <td>Comments</td>
      <td>💡 <code>:bulb:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>Initial commit</td>
      <td>🎉 <code>:tada:</code></td>
      <td><code>init</code></td>
    </tr>
    <tr>
      <td>Configuration</td>
      <td>🔧 <code>:wrench:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>Deploy</td>
      <td>🚀 <code>:rocket:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Documentation</td>
      <td>📚 <code>:books:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>In progress</td>
      <td>🚧 <code>:construction:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>UI Styling</td>
      <td>💄 <code>:lipstick:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Infrastructure</td>
      <td>🧱 <code>:bricks:</code></td>
      <td><code>ci</code></td>
    </tr>
    <tr>
      <td>Task List</td>
      <td>🔜 <code>:soon:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Move/Rename</td>
      <td>🚚 <code>:truck:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>New feature</td>
      <td>✨ <code>:sparkles:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Package.json in JS</td>
      <td>📦 <code>:package:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Performance</td>
      <td>⚡ <code>:zap:</code></td>
      <td><code>perf</code></td>
    </tr>
    <tr>
      <td>Refactor</td>
      <td>♻️ <code>:recycle:</code></td>
      <td><code>refactor</code></td>
    </tr>
    <tr>
      <td>Code Cleanup</td>
      <td>🧹 <code>:broom:</code></td>
      <td><code>cleanup</code></td>
    </tr>
    <tr>
      <td>Removing a file</td>
      <td>🗑️ <code>:wastebasket:</code></td>
      <td><code>remove</code></td>
    </tr>
    <tr>
      <td>Removing a dependency</td>
      <td>➖ <code>:heavy_minus_sign:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Responsiveness</td>
      <td>📱 <code>:iphone:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Reverting changes</td>
      <td>💥 <code>:boom:</code></td>
      <td><code>fix</code></td>
    </tr>
    <tr>
      <td>Security</td>
      <td>🔒️ <code>:lock:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>SEO</td>
      <td>🔍️ <code>:mag:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Version tag</td>
      <td>🔖 <code>:bookmark:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Approval Test</td>
      <td>✔️ <code>:heavy_check_mark:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Tests</td>
      <td>🧪 <code>:test_tube:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Text</td>
      <td>📝 <code>:pencil:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Typing</td>
      <td>🏷️ <code>:label:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Error Handling</td>
      <td>🥅 <code>:goal_net:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Data</td>
      <td>🗃️ <code>:card_file_box:</code></td>
      <td><code>raw</code></td>
    </tr>
  </tbody>
</table>

## 💻 Examples

<table>
  <thead>
    <tr>
      <th>Git Command</th>
      <th>GitHub Result</

th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>git commit -m "🎉 Initial commit"</code></td>
      <td>🎉 Initial commit</td>
    </tr>
    <tr>
      <td><code>git commit -m "💡 Fix typo in documentation"</code></td>
      <td>💡 Fix typo in documentation</td>
    </tr>
    <tr>
      <td><code>git commit -m "✨ Add user profile page"</code></td>
      <td>✨ Add user profile page</td>
    </tr>
    <tr>
      <td><code>git commit -m "🧹 Remove commented-out code"</code></td>
      <td>🧹 Remove commented-out code</td>
    </tr>
  </tbody>
</table>