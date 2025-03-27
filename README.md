# SimBreviloquentDemo

[![Deploy to GitHub Pages](https://github.com/1090MHz/SimBreviloquentDemo/actions/workflows/main.yml/badge.svg)](https://github.com/1090MHz/SimBreviloquentDemo/actions/workflows/main.yml)

This repository contains a Blazor WebAssembly demo project. The application is deployed to GitHub Pages and demonstrates the use of Blazor for building interactive web applications.

## Prerequisites

Before you begin, ensure you have the following installed on your system:
- [.NET SDK 9.0](https://dotnet.microsoft.com/download/dotnet/9.0)
- A code editor like [Visual Studio Code](https://code.visualstudio.com/) or [Visual Studio](https://visualstudio.microsoft.com/)

## Getting Started

Follow these steps to run the project locally:

### 1. Clone the Repository
```bash
git clone https://github.com/1090MHz/SimBreviloquentDemo.git
cd SimBreviloquentDemo
```

### 2. Restore Dependencies
Restore the required NuGet packages:
```bash
dotnet restore
```

### 3. Build the Project
Build the project to ensure everything is working:
```bash
dotnet build
```

### 4. Run the Project Locally
Run the project and serve it locally:
```bash
dotnet run
```
The application will be available at `http://localhost:5000` (or `https://localhost:5001` for HTTPS).

### 5. Publish the Project
To publish the project for deployment (e.g., to GitHub Pages):
```bash
dotnet publish -c Release -o release
```

## Deployment

This project is configured to deploy to GitHub Pages using a GitHub Actions workflow. The deployment process:
1. Builds the Blazor WebAssembly project.
2. Updates the `<base>` tag in `index.html` to match the GitHub Pages subdirectory.
3. Deploys the `wwwroot` folder to the `gh-pages` branch.

To trigger a deployment, push changes to the `main` branch. The workflow will automatically run and deploy the application.

## Project Structure

- `wwwroot/`: Contains static assets like CSS, JavaScript, and the Blazor WebAssembly files.
- `.github/workflows/main.yml`: GitHub Actions workflow for deploying to GitHub Pages.
- `SimBreviloquentDemo.csproj`: The project file for the Blazor WebAssembly application.

## Additional Commands

### Clean the Project
To clean the build artifacts:
```bash
dotnet clean
```

### Run Unit Tests
If the project includes unit tests, you can run them with:
```bash
dotnet test
```

## Resources

- [Blazor Documentation](https://learn.microsoft.com/en-us/aspnet/core/blazor/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)

---

Feel free to contribute to this project by submitting issues or pull requests!
