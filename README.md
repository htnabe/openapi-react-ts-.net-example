# OpenAPI-React-TypeScript-.NET-Example
This repository is an example of a project using TypeScript, React on the front, and .NET Web API, OpenAPI, Swagger on the back.

## Installation
```
git clone https://github.com/htnabe/OpenAPI-React-TypeScript-.NET-Example.git
```

### How to start

> [!IMPORTANT]
> `devcontainer` is available. If you failed to start the project by the following way, you can use this.

#### Using Task (recommended)

Install [go-task](https://taskfile.dev/installation/) if not already installed:
```
brew install go-task/tap/go-task
```

Start both frontend and backend simultaneously:
```
task
```

Or start each separately:
```
task front:dev   # Vite dev server
task back:dev    # dotnet watch
```

Available tasks:
| Command | Description |
|---|---|
| `task` | Start frontend + backend simultaneously |
| `task front:dev` | Start Vite dev server only |
| `task back:dev` | Start dotnet watch only |
| `task front:install` | Install npm packages |
| `task front:build` | Build frontend |
| `task back:build` | Build backend |

#### Manual

- Web API Server
```
cd webapi
dotnet restore
dotnet watch run
```

- Web App
```
cd front
npm install
npm run dev
```

Then,
- web app: `localhost:5173`
- web api: `localhost:5200`
