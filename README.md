# template_download_devdocs

## Usage

1. **Use this template** → Create a new repository
2. **Configure** your docs list (optional)
3. **Run workflow** manually from Actions tab
4. **Download** generated documentation from Releases

## Default Documents

By default, this workflow downloads:
- html
- css  
- javascript
- http

## Customization

### Option 1: Repository Variable (Recommended)
1. Go to Repository Settings → Secrets and variables → Actions → Variables
2. Add a new variable named `DOCS_USER`
3. Set value (comma-separated): `bash,git,python@3.12`

### Option 2: Manual Input
When running the workflow manually, you can specify a custom list in the "custom_docs_list" field.

### Option 3: Edit Workflow File
Modify the default value in `.github/workflows/create-release.yml`: