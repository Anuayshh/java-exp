# java-exp
# SIMPLE CALCULATOR USING REACT JS
# AIM:
To create a simple calculator using react js

# SOFTWARE:
Visual Studio Code

# ALGORITHM:
Set up the React environment: Install Node.js and create a new React project using create-react-app. Open your terminal or command prompt and run the following commands
Open the project in your preferred code editor.
Replace the contents of 'src/App.js" with the following code
Replace the contents of "src/App.css" with the following CSS styles
Start the development server: In the terminal, run npm start to start the React development server.
Open your browser and visit http://localhost:3000 to see the calculator.
# PROGRAM:
# APP.JS
java<br>
import React, { useState } from 'react';<br>
import './App.css';<br>

function App() {<br>
  const [result, setResult] = useState('');<br>

  const handleClick = (value) => {<br>
    setResult(result + value);<br>
  };<br>

  const calculate = () => {<br>
    try {<br>
      setResult(eval(result).toString());<br>
    } catch (error) {<br>
      setResult('Error');<br>
    }<br>
  };<br>

  const clear = () => {<br>
    setResult('');<br>
  };<br>

  return (<br>
    <div className="App"><br>
      <br></br>
      <br></br>
      <h2><u>SIMPLE CALCULATOR</u></h2><br>
      <br></br><br>
      <div className="calculator"><br>
        <input type="text" value={result} readOnly /><br>
        <div className="keypad"><br>
          <button onClick={() => handleClick('9')}>9</button><br>
          <button onClick={() => handleClick('8')}>8</button><br>
          <button onClick={() => handleClick('7')}>7</button><br>
          <button onClick={() => handleClick('6')}>6</button><br>
          <button onClick={() => handleClick('5')}>5</button><br>
          <button onClick={() => handleClick('4')}>4</button><br>
          <button onClick={() => handleClick('3')}>3</button><br>
          <button onClick={() => handleClick('2')}>2</button><br>
          <button onClick={() => handleClick('1')}>1</button><br>
          <button onClick={() => handleClick('+')}>+</button><br>
          <button onClick={() => handleClick('0')}>0</button><br>
          <button onClick={() => handleClick('-')}>-</button><br>
          <button onClick={() => handleClick('*')}>*</button><br>
          <button onClick={clear}>C</button><br>
          <button onClick={() => handleClick('/')}>/</button><br>
          <button onClick={() => handleClick('.')}>.</button><br>
          <button onClick={calculate}>=</button><br>
  </div><br>
      </div><br>
    </div><br>
  );<br>
}<br>

export default App;<br>
# APP.CSS:
java<br>
.App {<br>
  text-align: center;<br>
}<br>

.calculator {<br>
  width: 200px;<br>
  margin: 0 auto;<br>
  padding: 35px;<br>
  border: 2px solid #f77e7e;<br>
  border-radius: 5px;<br>
  
}<br>

input[type='text'] {<br>
  width: 100%;<br>
  margin-bottom: 20px;<br>
  padding: 5px;<br>
  font-size: 16px;<br>
}<br>

.keypad button {<br>
  width: 50px;<br>
  height: 30px;<br>
  margin: 2px;<br>
  font-size: 16px;<br>
  cursor: pointer;<br>
}<br>
# OUTPUT:
# IDLE:
![image](https://github.com/Anuayshh/java-exp/assets/127651217/dd71aa79-7309-4da8-bfe1-0a13a3d1c8db)

# CALCULATION:
![image](https://github.com/Anuayshh/java-exp/assets/127651217/413b5ea9-6256-4439-8cdc-ad9f0e56136f)
![image](https://github.com/Anuayshh/java-exp/assets/127651217/5923b0d1-493b-432a-b14d-1ebcc5be8ff7)


# RESULT:
Thus the simple calculator using react js.
