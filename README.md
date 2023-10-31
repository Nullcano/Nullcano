```
function makeReadMe(user) {
  const { username, name, bio, followers, following, publicRepos } = user

  const readmeContent = `
# ${name ? name : username}

${bio ? bio : 'Their past is a mystery, their silence unsettling.'}

## GitHub Stats
- Username: ${username}
- Followers: ${followers}
- Following: ${following}
- Public Repositories: ${publicRepos}
  `;

  return readmeContent
}

const user = users.find(user => user.name == 'Nullcano')

makeReadMe(user)
```
