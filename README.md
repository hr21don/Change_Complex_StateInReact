# Change_Complex_StateInReact

## Example Code
```
import React, { useState } from "react";

function App() {
  const [fName, setfName] = useState("");
  const [lName, setlName] = useState("");

  function update_F_name(event) {
    const firstname = event.target.value;
    setfName(firstname);
  }
  function update_L_name(event) {
    const lastname = event.target.value;
    setlName(lastname);
  }
  return (
    <div className="container">
      <h1>
        Hello {fName} {lName}
      </h1>
      <form>
        <input
          name="fName"
          onChange={update_F_name}
          placeholder="First Name"
          value={fName}
        />
        <input
          name="lName"
          onChange={update_L_name}
          placeholder="Last Name"
          value={lName}
        />
        <button>Submit</button>
      </form>
    </div>
  );
}

export default App;



```

## Input

Type Your Name into the 'First Name' and 'Last Name' text fields.

<img width="179" alt="Capture" src="https://user-images.githubusercontent.com/91548582/143574830-f834d037-be64-43e9-b377-61be43dcd604.PNG">

## Output

The example output for the app should look like this...|| Get in touch if you have trouble launching the app!

<img width="217" alt="Capture" src="https://user-images.githubusercontent.com/91548582/143574941-ec6e02b7-5cf4-4bac-ba3e-875e82106b60.PNG">
