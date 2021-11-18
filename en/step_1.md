In the Inspector window for the GameObject, click ‘Add Component’ and choose ‘New script’ then give your script a sensible name.

Double-click on your new script to open it in the code editor.

Create a variable to control the 'spinSpeed' 

```
float spinSpeed = 5.0f; //Change this number to spin faster or slower
```

Add code to spin your GameObject:

```
// Update is called once per frame
void Update()
{
    transform.Rotate(Vector3.up * spinSpeed); // rotate about the Y (up) axis
}
```

You can rotate about the X, Y, or Z axes by amending the direction in your code:
+ Vector3.right / Vector3.left = Rotation about the X axis
+ Vector3.up / Vector3.down = Rotation about the Y axis
+ Vector3.forward / Vector3.back = Rotation about the Z axis

![The Game view showing a hear GameObject spinning about it's Y axis.](images/spinning-heart.gif)

**Tip:** If you have added a 'Particle System' to your GameObject change the 'Simulation Space' property in the Inspector window to `World` so that it does not spin with your GameObject.
