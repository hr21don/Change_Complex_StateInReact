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
