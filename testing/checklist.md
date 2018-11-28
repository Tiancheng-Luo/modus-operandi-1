Testing
  On Windows, Linux, and OSX do

  Loads extension
  Loads LangaugeServer
    using PDK as source
    using Puppet-Agent as source
    using STDIO
    using TCP
      using local langserver
      using remote langserver
  Configuration
    debugFilePath
    featureFlags
    logLevel
    protocol
    tcp
      address
      port
    timeout
    format.enable
    installDirectory
    installType
  Functionality
    Syntax highlighting
    Hover
    Autocomplete
    Outline View
    Breadcrumbs
    Go to Symbol
    Linting (errors warning show in problems pane)
  Features
    Format document works (note some formatting not done by puppet-lint)
    Node Graph works with example manifest
    Puppet Resource user works
    PDK (note these are shell execs so unlikely to break)
      new module
      new class
      validate
      test unit
  Debug Adapter
    *This can't be autoamted at the moment, and is experimental so is not part of our test run right now*
  Command pallate
    Restart Current Session
    Show Connection Logs
    PDK New Module
    PDK Test Unit
    PDK Validate
    PDK New Task
    Puppet Resource
    Open Node Graph to the Side
  UI Button
    PDK new module
  Context Menu
    PDK New Module
    PDK Test Unit
    PDK Validate
    PDK New Task
    Puppet Resource
    Open Node Graph to the Side
