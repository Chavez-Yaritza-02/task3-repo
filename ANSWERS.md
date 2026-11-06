# Task 3 - Answers

1. `visible` decides if the modal is open or hidden. I used `useState` so pressing the share button can change that value and update the screen.

2. `onRequestClose` is for actions like pressing Back on Android. I call `closeModal` there because otherwise my modal would not close correctly with that button.

3. With `transparent={true}`, the profile stays visible behind the dark background of the modal. The available animations are `none`, `slide` and `fade`; I chose `fade`.

4. `ScrollView` lets me move around when there is more content than fits on the phone. With a normal `View`, the extra content could be cut off. For a much bigger list I would use `FlatList`, since it doesn't have to render every item at once.

5. `style` changes the scroll area itself. `contentContainerStyle` changes how the content is arranged inside it, for example the spacing between project cards.

6. `SafeAreaView` helps keep the app away from the notch, status bar and bottom system controls. I imported it from `react-native-safe-area-context` to work with the safe areas on different phones.

7. I kept one modal for sharing, used short lists and wrapped the screen in `SafeAreaView`. I wouldn't use a modal for a long form with several pages; that would be easier to complete on a separate screen.
