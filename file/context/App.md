import React from 'react';
import { ThemeProvider } from './ThemeContext';
import { UserProvider } from './UserContext.jsx';
import { CounterProvider } from './CounterContext.jsx';
import ThemedComponent from './ThemedComponent.jsx';
import UserComponent from './UserComponent.jsx/index.js';
import CounterComponent from './CounterComponent.jsx';

function App() {
  return (
    <ThemeProvider>
      <UserProvider>
        <CounterProvider>
          <div style={{ padding: '20px' }}>
            <ThemedComponent />
            <UserComponent />
            <CounterComponent />
          </div>
        </CounterProvider>
      </UserProvider>
    </ThemeProvider>
  );
}

export default App;