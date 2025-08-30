# Contributing Guidelines

Thank you for considering contributing to this project! 🎉  
We welcome contributions of all kinds – code, documentation, testing, ideas, and feedback.  

## How to Contribute

### 1. Fork & Clone
- Fork the repository to your GitHub account.
- Clone your fork locally:
  ```bash
  git clone https://github.com/juliettegodyere/Cook4Me.git
  cd Cook4Me
  ```

  ### 2. Create a Branch
  Create a new branch for your work:

  ```bash
  git checkout -b feature/your-feature-name
  ```

  _ Branch naming conventions:
  - feature/... → new features
  - fix/... → bug fixes
  - docs/... → documentation updates
  - chore/... → build/tooling changes

  ### 3. Install Dependencies

  #### Install Frontend (Expo with EAS) dependencies
```bash
cd frontend
# Install dependencies
yarn install   # or npm install

# Run locally with Expo
npx expo start

# For EAS builds (iOS/Android)
# Make sure you have EAS CLI installed globally
npm install -g eas-cli

# Configure project
eas build:configure

# Run build for Android
eas build -p android

# Run build for iOS
eas build -p ios
```

#### Install Backend (Spring Boot) dependencies
```bash
cd backend
# If using Maven
./mvnw clean install
./mvnw spring-boot:run

# If using Gradle
./gradlew build
./gradlew bootRun
```

### 4. Make Your Changes
    - Follow existing code style and structure.
    - Add comments for clarity where needed.
    - Update documentation (docs/) if your changes affect usage.

### 5. Run Tests
    - Ensure that all tests pass before submitting your PR.
    - Add new tests if you are adding new functionality.

### 6. Commit & Push Changes
Write clear commit messages:
```bash
git add .
git commit -m "feat: add authentication flow to frontend"
git push origin feature/my-feature
```
[Use Conventional Commits:] (https://www.conventionalcommits.org/en/v1.0.0/)

- feat: → new feature
- fix: → bug fix
- docs: → documentation
- chore: → maintenance

### 7. Push & Open a PR
Push your branch:
```bash
git push origin feature/your-feature-name
```
- Go to the repository on GitHub and click "New Pull Request".
- Clearly describe the changes you’ve made and why.
- Reference related issues if applicable (Fixes #123).
- Then open a Pull Request (PR) against the `main` branch.

### 8. Review & Merge
    - Your PR will be reviewed by maintainers.
    - Please be open to feedback and requested changes.
    - Once approved, it will be merged into main.

## Code of Conduct
We follow the [Contributor Covenant](https://www.contributor-covenant.org/).
Please be respectful and collaborative in all interactions.

## Good Practices

    - Keep PRs small and focused.
    - Document new functions, components, or endpoints.
    - Update relevant docs in /docs if your change affects architecture, APIs, or database schema.
    - Write meaningful commit messages:
        - `feat: add new booking API endpoint`
        - `fix: correct null pointer issue in user service`
        - `docs: update contributing guide`

fix: correct null pointer issue in user service

docs: update contributing guide

## Need Help
If you have questions:
- [Open an issue](https://github.com/juliettegodyere/Cook4Me.git/issues/new)
- Or reach out via [Discussions](https://github.com/juliettegodyere/Cook4Me.git/discussions) (if enabled)

Happy coding 🚀