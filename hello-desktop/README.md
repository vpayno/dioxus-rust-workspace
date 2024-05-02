# Development

Run the following command in the root of the project to start the Dioxus dev server:

```bash { background=false category=setup closeTerminalOnSuccess=true excludeFromRunAll=true interactive=true interpreter=bash name=hello-desktop-watch promptEnv=true terminalRows=10 }
dx serve --hot-reload --platform desktop
```

## Add project dependencies

```bash { background=false category=setup closeTerminalOnSuccess=true excludeFromRunAll=true interactive=true interpreter=bash name=hello-desktop-add-deps promptEnv=true terminalRows=10 }
pwd

sudo nala install -y --no-autoremove libwebkit2gtk-4.0-dev build-essential curl wget libssl-dev libgtk-3-dev libappindicator3-dev librsvg2-dev
sudo nala install -y --no-autoremove libsoup-3.0-dev libwebkit2gtk-4.1-dev libxdo-dev

printf "\n"

cargo add chrono --features serde
cargo add futures
cargo add reqwest --features json
cargo add serde --features derive
cargo add serde_json
cargo add async_recursion
cargo add serde --features derive
cargo add serde_json
```
