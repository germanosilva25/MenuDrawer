Agora, cada tela deve ser criada em arquivos separados dentro da pasta `screens`. Crie os seguintes arquivos:

### `index.js`
```javascript
import React from "react";
import { createDrawerNavigator } from "@react-navigation/drawer";
import { NavigationContainer } from "@react-navigation/native";
import HomeScreen from "./screens/HomeScreen";
import ProfileScreen from "./screens/ProfileScreen";
import SettingsScreen from "./screens/SettingsScreen";
import OrdersScreen from "./screens/OrdersScreen";
import PostsScreen from "./screens/PostsScreen";

// Criando o menu Drawer
const Drawer = createDrawerNavigator();

const DrawerMenu = () => (
  <Drawer.Navigator>
    <Drawer.Screen name="Home" component={HomeScreen} />
    <Drawer.Screen name="Profile" component={ProfileScreen} />
    <Drawer.Screen name="Settings" component={SettingsScreen} />
    <Drawer.Screen name="Orders" component={OrdersScreen} />
    <Drawer.Screen name="Posts" component={PostsScreen} />
  </Drawer.Navigator>
);

export default function App() {
  return (
    <NavigationContainer>
      <DrawerMenu />
    </NavigationContainer>
  );
}

```

### `screens/HomeScreen.js`
```javascript
import React from "react";
import { View, Text } from "react-native";

const HomeScreen = () => (
  <View style={{ flex: 1, justifyContent: "center", alignItems: "center" }}>
    <Text>Página Inicial</Text>
  </View>
);

export default HomeScreen;
```

### `screens/ProfileScreen.js`
```javascript
import React from "react";
import { View, Text } from "react-native";

const ProfileScreen = () => (
  <View style={{ flex: 1, justifyContent: "center", alignItems: "center" }}>
    <Text>Perfil</Text>
  </View>
);

export default ProfileScreen;
```

### `screens/SettingsScreen.js`
```javascript
import React from "react";
import { View, Text } from "react-native";

const SettingsScreen = () => (
  <View style={{ flex: 1, justifyContent: "center", alignItems: "center" }}>
    <Text>Configurações</Text>
  </View>
);

export default SettingsScreen;
```

### `screens/OrdersScreen.js`
```javascript
import React from "react";
import { View, Text } from "react-native";

const OrdersScreen = () => (
  <View style={{ flex: 1, justifyContent: "center", alignItems: "center" }}>
    <Text>Pedidos</Text>
  </View>
);

export default OrdersScreen;
```

### `screens/PostsScreen.js`
```javascript
import React from "react";
import { View, Text } from "react-native";

const PostsScreen = () => (
  <View style={{ flex: 1, justifyContent: "center", alignItems: "center" }}>
    <Text>Posts</Text>
  </View>
);

export default PostsScreen;
```

Isso mantém o código mais organizado. Me avise se precisar de mais ajustes! 🚀