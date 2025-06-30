# Alpine Linux Development Environment

This is an example Alpine Linux project used in Daytona.

[Try it out](https://daytona.io/#https://github.com/daytonaio-templates/base-alpine)

## Environment Variables

This project includes environment variable configuration to customize your development environment. The environment variables are automatically loaded into the devcontainer when you start your development environment.

### Setup

1. Copy the example environment file:
   ```bash
   cp .env.example .env
   ```

2. Modify the values in `.env` to match your preferences

3. Restart your devcontainer to apply the changes

### Available Environment Variables

#### System Configuration

- **ALPINE_VERSION**: Specifies the Alpine Linux version (default: `3.18`)
  - Used to ensure consistency across development environments

- **TIMEZONE**: Sets the system timezone (default: `UTC`)
  - Example: `America/New_York`, `Europe/London`, `Asia/Tokyo`

- **LANG**: Defines the system locale (default: `en_US.UTF-8`)
  - Controls language and character encoding settings

#### Shell and Editor Configuration

- **EDITOR**: Default text editor for command-line operations (default: `vi`)
  - Common alternatives: `nano`, `vim`, `emacs`

- **SHELL**: Default shell for the environment (default: `/bin/ash`)
  - Alpine Linux uses ash by default; alternatives include `/bin/bash` if installed

#### Development Environment

- **NODE_ENV**: Application environment mode (default: `development`)
  - Common values: `development`, `production`, `test`

- **DEBUG**: Enable debug output for applications (default: `false`)
  - Set to `true` to enable verbose logging in debug-aware applications

- **LOG_LEVEL**: Controls logging verbosity (default: `info`)
  - Common levels: `error`, `warn`, `info`, `debug`, `trace`

#### Optional Variables

The `.env.example` file also includes commented examples for common development variables like `PORT`, `HOST`, `DATABASE_URL`, `API_KEY`, and `CACHE_TTL`. Uncomment and configure these as needed for your specific project requirements.

### Want to contribute?

Feel free to [open a PR](https://github.com/daytonaio-templates/base-alpine) with any suggestions for this test project 😃 
