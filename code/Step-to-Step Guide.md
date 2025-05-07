# Step-by-Step Guide to Build the Ball Bounce App

Follow these steps to create the Ball Bounce app using **MIT App Inventor**:

---

## 1. Setting Up the Project
1. Open [MIT App Inventor](https://appinventor.mit.edu/).
2. Create a new project and name it `BallBounceApp`.

---

## 2. Designing the User Interface
1. **Add a Canvas**:
   - Drag a **Canvas** component from the **Drawing and Animation** palette onto the screen.
   - Set the Canvas properties:
     - **Width**: `Fill Parent`
     - **Height**: `Fill Parent`
   - This acts as the area where the ball will move.

2. **Add a Ball**:
   - Drag a **Ball** component onto the Canvas.
   - Set its properties:
     - **Radius**: `10`
     - **Color**: Choose a bright color (e.g., green).

---

## 3. Adding the Code Logic
1. Switch to the **Blocks Editor**.
2. Add the following blocks:

   ### **a. Fling Event**
   - Drag the `when Ball1.Flung` block from the Ball component.
   - Inside this block:
     1. Add `set Ball1.Heading to get heading` to make the ball move in the direction of the fling.
     2. Add `set Ball1.Speed to 100` to set the ball's speed.

   ### **b. Edge Reached Event**
   - Drag the `when Ball1.EdgeReached` block from the Ball component.
   - Inside this block:
     1. Add `call Ball1.Bounce edge` to make the ball bounce back upon hitting an edge.

---

## 4. Testing the App
1. Connect your mobile device or emulator to MIT App Inventor.
2. Test the app by flinging the ball in different directions and observing how it bounces upon hitting the edges.

---

## Example Code Blocks
```plaintext
When Ball1.Flung
    Set Ball1.Heading to get heading
    Set Ball1.Speed to 100

When Ball1.EdgeReached
    Call Ball1.Bounce edge
