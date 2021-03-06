# Troubleshooting

If you are having trouble with Stoplight Platform and cannot find an answer in the documentation, see if this page can help, then [contact support](mailto:support@stoplight.io) if not.

## Browser Support

We aim to support the following browsers and minimum versions. 

|               | Chrome | Safari                   | Firefox | Edge                     |
|---------------|--------|--------------------------|---------|--------------------------|
| Documentation | 68     | 12                       | 60      | 18                       |
| Platform      | 68     | 12                       | 60      | Not Supported            |
| Studio Web    | 75     | Not Supported            | 68      | Not Supported            |

Things may work outside of these browsers and these versions, but there might be unexpected problems as we won't be testing those environments.

If something is not working in a version listed here (or newer) please [contact support](mailto:support@stoplight.io).

## Can't Edit Project in Studio

#### Not a Git project and I'm the owner

Local projects in Stoplight are stored in the browser cache. If you are on a different computer/browser, you won't be able to edit the project. 

Preferably [connect to a Git provider](2.-workspaces/e.configure-git.md) that Stoplight supports. Once you've done that go into studio from the browser/computer you used to first create this project, and then promote it to a Git repo.

![Promote to Git](assets/images/git_promote.png)

The Git integration will allow you and your team members (Makers and above) to collaborate on this project. Keep in mind that they would need access to the Git repository as well. Git repositories are very useful once other stakeholders such as developers need access to the API designs and they support a formal review process for your design or documentation workflows via merge requests.

If you can't use a Git provider you'd be limited to using the project from the same browser you first created it from. 

**Note**: Other users in your workspace won't be able to edit a local project.

#### I'm the on the same browser/computer

This could be because you recently updated or cleaned the cache of your browser. In that case you can export the OpenAPI and schemas using the export button available in the docs. Then, import the exported files into a new project and promote it to a git project.

![Export to OpenAPI](assets/images/export-openapi.png)

## Can't find GitHub Organization 

This could be due to missing permissions in GitHub. Navigate to https://github.com/settings/applications and find the Stoplight app. Click on it to go into the settings.

![GitHub Organization Access](assets/images/organization-access.png)

Notice the organization access at the bottom. Grant access to the organization you're looking to add repos from. You should then be able to add projects from your organization.

