# Course Specification: Maya's Mechanical Magic

## 1. Core Technical Architecture
- **Framework:** Single Page Application (SPA) using dynamic, state-driven JavaScript view updates.
- **UI Design:** Dark slate theme (bg-slate-900) with high-contrast accent highlights (Amber for system elements, Cyan for strings, Emerald for numbers, Purple for logic).
- **Execution Sandbox:** Skulpt (client-side JavaScript-based Python 3 interpreter).
- **Audio Delivery:** Native Web Speech API (window.speechSynthesis). The system must call window.speechSynthesis.cancel() immediately before loading any new text to prevent audio overlapping.
- **Error Interception:** Intercept standard Python exceptions and format them inside a clean alert container: ❌ Mistake in the recipe: [Simplified Error String].

---

## 2. The 14-Lesson Curriculum Matrix

### 📦 Module 1: The Workshop Foundations

#### Lesson 1: The print() Command
- **Concept:** Telling the computer to display a message on the screen.
- **Image Prompt:** Maya typing on an antique typewriter connected to a massive glowing book labeled 'Magic Python Recipe Book'. A tiny clockwork robot (Cog-Bot) boots up on the workbench in a soft blue glow. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** Welcome to the workshop! Coding isn't mystery magic—it's just a recipe book of clear instructions. When Maya types a command like 'print' into the magic book, the workshop listens and makes things happen. Try running the code to say hello to Cog-Bot!
- **Starter Code:**
```python
print("Hello, Cog-Bot!")
```

#### Lesson 2: String Variables
- **Concept:** Storing words inside labeled memory containers.
- **Image Prompt:** Maya organizing translucent, glowing data boxes on a workshop storage rack. A blue box labeled 'robot_name' holds floating neon text. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** To help our robot remember things, Maya uses magic storage boxes called variables. Each box gets a clear label and stores one piece of information, like a name. Let's see what name is currently inside our box!
- **Starter Code:**
```python
robot_name = "Cog-Bot"
print("The robot's name is:")
print(robot_name)
```

#### Lesson 3: Number Variables & Math
- **Concept:** Storing integers and using operators (+, -, *, /) for calculations.
- **Image Prompt:** Maya dropping glowing green metal spheres into a mechanical counting bin labeled 'bolt_count' on the workbench. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** Variables can store numbers too! Maya can count her spare parts and use math to see how many total pieces she has available. Let's add our storage boxes together.
- **Starter Code:**
```python
box_a = 10
box_b = 5
total_bolts = box_a + box_b
print("Total bolts in workshop:")
print(total_bolts)
```

#### Lesson 4: User Input
- **Concept:** Pausing the program to let the user type information.
- **Image Prompt:** Maya typing into a glowing headset controller to send a message directly to Cog-Bot's digital chest screen. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** Let's make the code a two-way street. We can use the 'input' command to talk directly to the program while it runs. Type your name into the box when it asks!
- **Starter Code:**
```python
pilot_name = input("Enter your name, Pilot: ")
print("Welcome to the control center, " + pilot_name)
```

---

### 🚦 Module 2: Making Decisions

#### Lesson 5: Simple IF Statements
- **Concept:** Running a block of code only if a specific condition is True.
- **Image Prompt:** A mechanical wall switch with a glowing copper wire running directly to a single light bulb over Cog-Bot's charging pad. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** An 'if' statement is like a mechanical switch. If the condition is true, the code inside runs. If it's false, the computer completely skips it! Try changing True to False to see what happens.
- **Starter Code:**
```python
switch_on = True
if switch_on == True:
    print("💡 The workshop lights turn on!")
```

#### Lesson 6: ELSE and ELIF Chains
- **Concept:** Handling multiple alternative choices in decision making.
- **Image Prompt:** A miniature indoor railway track splitting into three different paths based on a color-changing signal post. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** What if a switch has more than two choices? We can use 'elif' and 'else' to create a multi-track railway for our logic to follow based on battery levels.
- **Starter Code:**
```python
battery_level = 20

if battery_level > 70:
    print("🔋 Battery is full!")
elif battery_level > 30:
    print("⚠️ Battery is getting low.")
else:
    print("🚨 Battery dead! Plug in immediately!")
```

#### Lesson 7: Complex Logic (AND)
- **Concept:** Combining multiple conditions using the 'and' operator.
- **Image Prompt:** A massive vault door with two separate heavy mechanical keyholes that must be turned at the exact same moment to open. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** Sometimes multiple conditions must be true at once. We use the word 'and' to connect them. Let's see if we have enough parts to unlock our flying drone blueprint!
- **Starter Code:**
```python
has_metal = True
bolt_count = 12

if has_metal == True and bolt_count >= 10:
    print("🚀 Blueprint unlocked! Building drone.")
else:
    print("❌ Missing parts.")
```

---

### 🔄 Module 3: Storage & Loops

#### Lesson 8: Python Lists
- **Concept:** Storing multiple indexed items inside a single variable container.
- **Image Prompt:** A wooden tool cabinet with numbered pull-out drawers holding different mechanical gadgets like hammers and wrenches. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** Instead of creating a separate box for every single item, we can use a list to store a whole row of tools inside one single variable cupboard!
- **Starter Code:**
```python
tools = ["Hammer", "Wrench", "Pliers"]
print("The item in drawer 0 is:")
print(tools[0])
```

#### Lesson 9: FOR Loops
- **Concept:** Iterating through each item in a list sequentially.
- **Image Prompt:** A horizontal neon laser scanner sliding down over the tool chest drawers one by one, lighting them up. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** A for loop lets us look at every single item inside a list automatically. The computer loops down the line so you don't have to write the print command over and over again.
- **Starter Code:**
```python
tools = ["Hammer", "Wrench", "Pliers"]
for item in tools:
    print("Scanning tool: " + item)
```

#### Lesson 10: WHILE Loops
- **Concept:** Repeating a code block continuously as long as a condition remains True.
- **Image Prompt:** A copper water pump looping water through a clear pipe continuously while a brass valve remains open. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** A while loop is like an engine that runs forever as long as its fuel switch stays True. We can use this to keep our program running non-stop!
- **Starter Code:**
```python
fuel = 3
while fuel > 0:
    print("⚙️ Engine running! Fuel left:", fuel)
    fuel = fuel - 1
print("🛑 Out of fuel. Stopping.")
```

---

### 🛠️ Module 4: Blueprints & Functions

#### Lesson 11: Simple Functions
- **Concept:** Bundling code blocks into reusable names using 'def'.
- **Image Prompt:** A heavy mechanical stamping press that leaves a uniform gear imprint on flat sheets of metal. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** Functions are custom blueprints. You group a collection of commands together under one short name, so you can perform a complex task instantly anywhere in your code.
- **Starter Code:**
```python
def boot_system():
    print("Initializing Core...")
    print("Waking up Cog-Bot...")
    print("🟢 System Ready!")

boot_system()
```

#### Lesson 12: Functions with Inputs
- **Concept:** Passing external arguments into functions to alter their calculations.
- **Image Prompt:** Maya feeding raw scrap metal into the side of a processing machine and watching custom-sized gear pieces pop out. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** We can pass data into our functions to customize how the blueprint works. Watch how the same function gives different results based on the number we feed it!
- **Starter Code:**
```python
def calculate_gears(iron):
    gear_count = iron * 3
    print("Gears made:", gear_count)

calculate_gears(5)
```

---

### 🏁 Module 5: Graduation Projects

#### Lesson 13: Capstone Crafting Calculator
- **Concept:** Combining loops, conditionals, variables, and dict structures into an interactive terminal app.
- **Image Prompt:** Maya standing proudly in front of a glowing control panel dashboard showing current inventory levels and active machine builds. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** Time for your final challenge! You are going to build a continuous command center using a loop. It keeps track of workshop materials and lets you choose whether to check your inventory stock or craft an item.
- **Starter Code:**
```python
inventory = {"iron": 15, "copper": 8}

def show_stock():
    print("\n📦 Iron:", inventory["iron"], "| Copper:", inventory["copper"])

running = True
while running:
    show_stock()
    action = input("Options: 1=Craft, 2=Exit -> ")
    if action == "1":
        if inventory["iron"] >= 5 and inventory["copper"] >= 4:
            print("✨ Successfully crafted a drone component!")
            inventory["iron"] -= 5
            inventory["copper"] -= 4
        else:
            print("❌ Not enough materials!")
    elif action == "2":
        print("Goodbye, Master Engineer!")
        running = False
```

#### Lesson 14: Desktop Graduation (VS Code)
- **Concept:** Transitioning from the browser playground to a local Python interpreter and VS Code environment.
- **Image Prompt:** Maya sitting at a clean, well-lit desk booting up a real laptop running VS Code with Cog-Bot sitting right next to the keyboard. 3D Pixar style animation, highly detailed, vibrant colors, volumetric warm workshop lighting, cinematic composition, claymation texture look, kid-friendly illustration.
- **Voice Text:** Congratulations! You have completed the browser training course. Now you're ready to use real professional tools on your computer. Follow the steps on your screen to download Python, install VS Code, and bring your code into the real world!
- **Starter Code:**
```python
# Follow the interactive checklist on the screen to set up your environment!
print("Master Inventor Status: Achieved.")
```
