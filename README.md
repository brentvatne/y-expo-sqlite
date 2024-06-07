# y-expo-sqlite

```js
import { ExpoSQLitePersistence } from "y-expo-sqlite";

const __ydoc = new Y.Doc();
const __yarray = __ydoc.getArray<Todo>("todos");

const provider = new ExpoSQLitePersistence("TodosDoc", __ydoc);
provider.whenSynced.then(() => {
  console.log("content finished loading from database.");
});
```