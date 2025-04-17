# Sahan_Beta-MD
©For Bot Asitha-Md


`Pair Device Whatsapp`
https://asitha.top/pair

*ඔයාගේ බොට් නම්බරේ ගහලා Login වෙන්න...*
(ex-94742314485)
Session Id ඒක ආවේ නැත්නම් පරණ ඒක Logout කරලා අලුතින් Session Id ගන්න... 🌚❤️



`Workflow code`
name: Node.js CI

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main

jobs:
  build:

    runs-on: ubuntu-latest

    strategy:
      matrix:
        node-version: [20.x]

    steps:
    - name: Checkout repository
      uses: actions/checkout@v3

    - name: Set up Node.js
      uses: actions/setup-node@v3
      with:
        node-version: ${{ matrix.node-version }}

    - name: Install dependencies
      run: npm install

    - name: Start application
      run: npm start

      

