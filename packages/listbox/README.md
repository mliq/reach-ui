# @reach/listbox

[![Stable release](https://img.shields.io/npm/v/@reach/listbox.svg)](https://npm.im/@reach/listbox) ![MIT license](https://badgen.now.sh/badge/license/MIT)

[Docs](https://reacttraining.com/reach-ui/listbox) | [Source](https://github.com/reach/reach-ui/tree/master/packages/listbox) | [WAI-ARIA](https://www.w3.org/TR/wai-aria-practices-1.1/#Listbox)

An accessible listbox for custom select inputs.

```jsx
import React, { useState } from "react";
import { Listbox, ListboxOption } from "@reach/listbox";
import "@reach/listbox/styles.css";

function Example(props) {
  let [value, setValue] = useState("default");
  return (
    <Listbox value={value} onChange={value => setValue(value)}>
      <ListboxOption value="default">🌮 Choose a taco</ListboxOption>
      <hr />
      <ListboxOption value="asada" valueText="Carne Asada">
        🌮 Carne Asada
      </ListboxOption>
      <ListboxOption value="pollo" valueText="Pollo">
        🌮 Pollo
      </ListboxOption>
      <ListboxOption value="pastor" valueText="Pastor">
        🌮 Pastor
      </ListboxOption>
      <ListboxOption value="lengua" valueText="Lengua">
        🌮 Lengua
      </ListboxOption>
    </Listbox>
  );
}
```
