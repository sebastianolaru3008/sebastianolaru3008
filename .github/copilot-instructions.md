# GitHub Profile README Repository

This is a special GitHub profile README repository (sebastianolaru3008/sebastianolaru3008) that displays content on the user's GitHub profile page. The repository contains only a README.md file that serves as the profile's main content.

Always reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.

## Working Effectively

### Repository Setup and Navigation
- Clone the repository: `git clone https://github.com/sebastianolaru3008/sebastianolaru3008.git`
- Navigate to repository: `cd sebastianolaru3008`
- Check repository status: `git status`
- View repository structure: `ls -la` (contains only README.md and .git directory)

### Essential Tools Installation
Install required validation tools before making changes:
- `npm install -g markdownlint-cli` -- takes 10-15 seconds to complete
- `npm install -g markdown-link-check` -- takes 10-15 seconds to complete

### Content Editing Workflow
- Edit the README.md file using any text editor
- Preview changes locally before committing
- Always validate markdown syntax and links before pushing changes

### Validation Commands
Run these validation commands after making any changes to README.md:

#### Markdown Linting
- `markdownlint README.md` -- takes 2-3 seconds to complete
- NOTE: This command will show style violations but may exit with code 1. This is normal for profile READMEs that use HTML badges and formatting.
- Common acceptable violations for profile READMEs:
  - MD033 (inline HTML) - badges and social links require HTML
  - MD013 (line length) - badge URLs are naturally long
  - MD041 (first line heading) - profile READMEs often start with greeting

#### Link Validation
- `markdown-link-check README.md` -- takes 10-20 seconds to complete
- NOTE: Link checking may fail due to network restrictions or external site policies. Status: 0 errors are common in sandboxed environments.
- Always test links manually in a browser when possible

#### Git Workflow Validation
- `git diff` -- shows changes made to files
- `git status` -- shows current working tree status
- `wc -l README.md` -- current file has 55 lines, use as baseline

## Repository Information

### Current Repository State
- **Type**: GitHub profile README repository
- **Primary file**: README.md (3,666 bytes, 55 lines)
- **Content**: Personal profile with social links, skills badges, and GitHub stats
- **Special behavior**: Content displays on https://github.com/sebastianolaru3008 profile page

### Repository Structure
```
sebastianolaru3008/
├── .git/
├── .github/
│   └── copilot-instructions.md (this file)
└── README.md
```

### Git Branches
- `master` - main branch with original content
- `copilot/fix-*` - working branches for changes

## Validation Scenarios

After making any changes to README.md:

1. **Syntax Validation**: Run `markdownlint README.md` to check markdown syntax
2. **Link Testing**: Run `markdown-link-check README.md` to verify links (note: may fail in restricted environments)
3. **Content Review**: Verify the README.md content is appropriate for a professional GitHub profile
4. **Length Check**: Ensure file size remains reasonable (`wc -l README.md` should be similar to baseline of 55 lines)
5. **Git Status**: Run `git status` and `git diff` to review changes before committing

## Common Tasks

### Updating Profile Content
- Edit social media links in the "Connect with me" section
- Update skills badges in the "Languages and Tools" section  
- Modify personal description and goals
- Always maintain professional tone and appropriate content

### Adding New Social Links
- Follow existing pattern using badge format from shields.io
- Test links before committing
- Maintain consistent styling with existing badges

### Testing Changes
- Use `git diff` to review changes
- Run validation commands listed above
- Preview markdown rendering if tools are available

## Important Notes

- **NO BUILD PROCESS**: This repository has no build steps, compilation, or deployment processes
- **NO TESTS**: There are no automated tests to run
- **NO DEPENDENCIES**: No package.json, requirements.txt, or other dependency files
- **PROFILE REPOSITORY**: Content appears on GitHub profile page at https://github.com/sebastianolaru3008
- **VALIDATION LIMITATIONS**: Link checking may fail in sandboxed environments due to network restrictions
- **HTML ALLOWED**: Markdown linting will flag HTML usage, but this is acceptable for GitHub profile READMEs that need badges and custom formatting

## Troubleshooting

### Link Check Failures
If `markdown-link-check` reports "Status: 0" errors:
- This is expected in restricted network environments
- Manually verify important links when possible
- Focus on fixing obvious broken links (typos, malformed URLs)

### Markdown Lint Warnings
Profile READMEs commonly have acceptable lint violations:
- Inline HTML for badges is normal and required
- Long lines due to badge URLs are acceptable
- Custom formatting for visual appeal is allowed

### Git Workflow Issues
- Always use `git status` to check current state
- Use `git diff` to review changes before committing
- Ensure you're on the correct working branch

## File Locations Reference

- **Main content**: `/README.md`
- **Instructions**: `/.github/copilot-instructions.md`
- **Repository root**: contains only essential files, no source code directories