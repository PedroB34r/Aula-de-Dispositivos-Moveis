# Aula-de-Dispositivos-Moveis
Codigos de React, JS e Jsom








import * as React from 'react';
import {StyleSheet, Text, View, TextInput, Button} from 'react-native';
import {NavigationContainer} from '@react-navigation/native';
import {createDrawerNavigator} from '@react-navigation/drawer';

/*  a const pode ser substituida por Function e seu nome tambem pode ser alterado*/
const Tab = createDrawerNavigator();

/*import {createBottomTabNavigator} from '@react-navigation/bottom-tabs';
const Tab = createBottomTabNavigator(); cria pequenos botoes*/


/** ao alterar o nomo da const pu function deve se alterar os nomes das Screen */
    const Atv1 = () => {
return(
  <NavigationContainer>
        <Tab.Navigator>
          <Tab.Screen name="Cadastrar" component={Cadastra}/>
          <Tab.Screen name="Listados" component={Listar}/>
        </Tab.Navigator>
      </NavigationContainer>
);
    }
    
    const Cadastra = () =>{
      return(
          <View>
            <Text>Nome</Text>
            <TextInput/>
            <Text>Telefone</Text>
            <TextInput/>
           <Button 
           title='Salvar'
           color="#BAC521"/>
            </View>
      );
    }

    const Listar = () =>{
      return(
        <View>
         <Text>
           Aiolos
           (11)92589-9878
           </Text>

           <Text>
           Aiolia
           (11)92589-9879
           </Text>
           
           <Text>
           Regulus
           (11)92589-9880
           </Text>
           
       </View>
      );
    }

export default Atv1; 

/*chaninho*/
