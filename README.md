# Micro Frontend Service

Installing node_modules:

`npm install`

Run host-app with using command:

`npm start`

### How to start micro service project from the split repository

1. You should rename all occurrences by name - mfServiceName to any name you need. 
2. Install dependencies by command 'yarn'.
3. Start your app by command 'yarn local' when you develop your app and by command 'yarn dev' when you check your connection with host app.  

### How to pass data between your apps 

You should use 'src/hostAppFiles/createDispatchEventToService' for call event and pass your data.
You should use 'src/hostAppFiles/useWindowEventListener' for subscribe event and get your data.

Don`t forget to unsubscribe from events when component will be unmounted.

### Applied Technology Stack

```
- React
- React app rewired
- Styled-components
- TypeScript
- Holism GPB UI
- ES Lint
- Prettier
```

### Available aliases

```
- @app          => root/src
- @assets       => root/src/assets
- @components   => root/src/components
- @constants    => root/src/constants
- @models       => root/src/models
- @service      => root/src/service
- @styles       => root/src/styles
```

### Branch naming rules

```
- feature/taskNumber-someDescription         => new development task
- bugfix/taskNumber-someDescription          => bug fix task in component
- hotfix/taskNumber-someDescription          => hotfix task in component
- release/releaseNumber                      => branch for deploy
```

For better understanding the micro frontend architecture follow the link on Medium:
[A Micro Frontend Solution for React](https://levelup.gitconnected.com/a-micro-frontend-solution-for-react-1914b19663b)
