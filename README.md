# React-Native-popup-modal

### Usage

```
<Root>
    <View>
        <TouchableOpacity
            onPress={() =>
              Popup.show({
              type: 'Survey', // Success, Survey, Danger, Warning
              /* image: require('./logo.png'), */  // optional
              title: 'New Survey',
              button: true,
              closebutton: true,
              closebuttonText: 'Close', // Default Close
              textBody: 'Would you like to participate in our survey ?',
              buttonText: 'Take the Survey',
              closeBtn: () => Popup.hide(),
              callback: () => {
                navigation.navigate("BusTime"),
                Popup.hide()
              }
            })
            }
        >
            <Text>Open Popup</Text>
        </TouchableOpacity>
    </View>
</Root>
```
Toast component

```
<Root>
    <View>
        <TouchableOpacity
            onPress={() => 
                    Toast.show({
                        type: 'Success', // Success, Warning, Danger
                        title: 'User created',
                        text: 'Your user was successfully created, use the app now.',
                        color: '#2ecc71'
                    })
          >
            <Text>Open Toast</Text>
        </TouchableOpacity>
    </View>
</Root>
```
