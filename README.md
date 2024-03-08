# Stock Backend
Simple API built in Elixir to fetch data required to calculate historic stock portfolio performance 

## Getting started 
* Install Elixir
  * Run the following command in terminal `brew update && brew install elixir`
* Build dependencies
  * Run `mix deps.get` once inside `/frontend/`
* Add Marketstack API Key as environment variable `MARKETSTACK_API_KEY`
  * for a temporary option run: `export MARKETSTACK_API_KEY=API_KEY_HERE`
  * for more permanent solution copy command above into your shell config e.g. `~\.zshrc or ~\.profile`
* Start the Phoenix server
  * run `mix phx.server`

Congrats! Your server should now be available on `localhost:4000`, you can try making a GET request to `localhost:4000/api/fetch-data` with the query params `symbols: string` (e.g. AAPL,NVDA) and `date_initial: string` e.g. ("2024-02-26")
