https://github.com/hyperspaceai/aios-cli


docker pull kartikhyper/aios

docker run -d kartikhyper/aios

docker exec -it CONTAINER-ID /bin/bash

apt install nano

nano priv.key

Usage: aios-cli [OPTIONS] <COMMAND>

Commands:
  start        Start the local daemon
  status       Check the status of your local daemon
  kill         Kills the currently running local daemon
  models       Manage your local models
  state        Manage the app state
  system-info  Get system information
  infer        Use local models to do inference
  hive         Run commands using the Hive servers
  version      Check the curent version
  help         Print this message or the help of the given subcommand(s)

./aios-cli models list

Found 1 models downloaded locally
  hf:second-state/Gemma-2b-it-GGUF:gemma-2b-it-Q4_K_M.gguf

Exemple:
./aios-cli infer --model hf:second-state/Gemma-2b-it-GGUF:gemma-2b-it-Q4_K_M.gguf --prompt "Explique comment gagner des points sur Hive."

./aios-cli hive import-keys priv.key
Successfully imported your keys

Usage: aios-cli hive [OPTIONS] <COMMAND>

Commands:
  login        Login with your keypair credentials
  import-keys  Import your keys (either v0 JSON or ed25519 PEM file)
  connect      Connect to the network and provide inference using local models
  registered   Get the list of models you're currently registered with
  reregister   Reregister any new models that have been added since the last time you connected
  whoami       Get currently signed in keys
  disconnect   Disconnect from the network
  infer        Run an inference on the network
  listen       Listen for all hive events
  interrupt    Interrupt an inference you are currently doing for the network
  select-tier  Pick a tier to opt-in to the points system
  allocate     Pick a tier by choosing how much VRAM you would like to allocate
  points       View your points earned and current multiplier
  help         Print this message or the help of the given subcommand(s)

Options:
      --verbose
  -h, --help     Print help

./aios-cli hive login
Using locally saved keys
Authenticated successfully!

root@5bb8fca062cb:/app# ./aios-cli hive whoami
Public: ********************************************
Private: ********************************************

./aios-cli hive registered
Found 1 models registered on hive
  hf:second-state/Gemma-2b-it-GGUF:gemma-2b-it-Q4_K_M.gguf

./aios-cli hive select-tier 3
Successfully running on tier: 3

./aios-cli hive points
Points: ********
Multiplier: 2.00

root@5bb8fca062cb:/app# ./aios-cli version
Version: 0.1.6

./aios-cli hive listen
Logs
](https://github.com/hyperspaceai/aios-cli


`docker pull kartikhyper/aios`

`docker run -d kartikhyper/aios`

`docker exec -it CONTAINER-ID /bin/bash`

`apt install nano`

`nano priv.key`

`Usage: aios-cli [OPTIONS] <COMMAND>

Commands:
  start        Start the local daemon
  status       Check the status of your local daemon
  kill         Kills the currently running local daemon
  models       Manage your local models
  state        Manage the app state
  system-info  Get system information
  infer        Use local models to do inference
  hive         Run commands using the Hive servers
  version      Check the curent version
  help         Print this message or the help of the given subcommand(s)`

`./aios-cli models list`

Found 1 models downloaded locally
  hf:second-state/Gemma-2b-it-GGUF:gemma-2b-it-Q4_K_M.gguf

Exemple
`./aios-cli infer --model hf:second-state/Gemma-2b-it-GGUF:gemma-2b-it-Q4_K_M.gguf --prompt "Explique comment gagner des points sur Hive."`

`./aios-cli hive import-keys priv.key`
Successfully imported your keys

`Usage: aios-cli hive [OPTIONS] <COMMAND>

Commands:
  login        Login with your keypair credentials
  import-keys  Import your keys (either v0 JSON or ed25519 PEM file)
  connect      Connect to the network and provide inference using local models
  registered   Get the list of models you're currently registered with
  reregister   Reregister any new models that have been added since the last time you connected
  whoami       Get currently signed in keys
  disconnect   Disconnect from the network
  infer        Run an inference on the network
  listen       Listen for all hive events
  interrupt    Interrupt an inference you are currently doing for the network
  select-tier  Pick a tier to opt-in to the points system
  allocate     Pick a tier by choosing how much VRAM you would like to allocate
  points       View your points earned and current multiplier
  help         Print this message or the help of the given subcommand(s)

Options:
      --verbose
  -h, --help     Print help`

`./aios-cli hive login`
Using locally saved keys
Authenticated successfully!

`./aios-cli hive whoami`
Public: ********************************************
Private: ********************************************

`./aios-cli hive registered`
Found 1 models registered on hive
  hf:second-state/Gemma-2b-it-GGUF:gemma-2b-it-Q4_K_M.gguf

`./aios-cli hive select-tier 3`
Successfully running on tier: 3

`./aios-cli hive points`
Points: ********
Multiplier: 2.00

`./aios-cli version`
Version: 0.1.6

`./aios-cli hive listen`
Logs

)
