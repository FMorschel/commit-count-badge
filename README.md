# Commit Count Badge

Generates a Shields.io badge for commit count in a specified repository.

## Inputs

- **repository** (required): The GitHub repository (user/project) to query commits from.
- **author** (required): The author whose commits should be counted.
- **text** (required): The label text for the badge.
- **outputPath** (required): Path and file name for the generated badge (e.g., 'badges/dart-commits.svg').
- **token** (required): GitHub token to authenticate API requests.
- **logo** (optional): The logo to include in the badge. Default is 'github'.
- **labelColor** (optional): The background color for the badge label. Default is '#0175C2'.
- **color** (optional): The background color for the badge value. Default is 'lightgray'.

## Example Usage

```yaml
uses: FMorschel/commit-count-badge@v1
with:
  repository: 'flutter/flutter'
  author: 'FMorschel'
  text: 'Flutter SDK Commits'
  outputPath: 'badges/flutter-commits.svg'
  token: '${{ secrets.GITHUB_TOKEN }}'
  logo: 'flutter'
  labelColor: '#00A9E0'
  color: 'lightgray'
```

## Description

This GitHub Action counts the number of commits made by a specified author in a repository and generates a Shields.io badge reflecting this count. The badge is saved to the specified output path within your repository.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Installation

### Add the Action to Your Workflow

Include the action in your workflow YAML file as shown in the example usage.

### Run the Workflow

The action can be triggered on a schedule or manually, depending on your workflow configuration.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

## Support

If you encounter any issues or have questions, feel free to open an issue in the repository.
