# ViewModel + Unidirectional Data Flow
CS 501 Midterm #2
Implemented the Counter Screen that has been refactored, so that state is managed by a ViewModel instead of the composable.

## Satisfies and Includes all the Requirements: 
Given Code
@Composable
fun CounterScreen() {
    var count by remember { mutableStateOf(0) }
    Column {
        Text("Count: $count")
        Button(onClick = { count++ }) {
            Text("Increment")
        }
    }
}

Modify the code so that:
1.	The counter state is stored inside a ViewModel
2.	The composable reads the state from the ViewModel
3.	Button presses call a ViewModel function
4.	The UI recomposes when the state changes

Requirements
You must create:
•	a CounterViewModel
•	a CounterScreen composable
