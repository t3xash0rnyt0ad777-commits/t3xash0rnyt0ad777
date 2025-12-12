# t3xash0rnyt0ad777
auto-modmail
name: Blockchain API Call

on:
  workflow_dispatch:

jobs:
  call-api:
    runs-on: ubuntu-latest
    steps:
      - name: Make API request
        run: |
          curl -X POST https://api.example.com/endpoint \
            -H "Authorization: Bearer ${{ secrets.API_TOKEN }}" \
            -H "Content-Type: application/json" \
            -d '{
              "address": "ex1qhrvfnvsxsummaqa7tsqp78dyl6qzvaly4cmcm3"
            }'
            https://mempool.space/tx/4112616ed31e14751d00113439b62464d54738326aeceff699f6f1d71187396e
