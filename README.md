<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Laboratory Work No. 1</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <h1>Laboratory Work No. 1</h1>

    <!-- Layout Table -->
    <table class="layout">
        <tr>
            <td>
                <h2>Computer Photo</h2>
                <img src="computer.png" alt="Atari Computer" width="150">
            </td>
            <td class="fixed-cell">
                <p>Block w=140</p>
            </td>
        </tr>
    </table>

    <!-- Bulleted List -->
    <h2>Favorite Things (Unordered List)</h2>
    <ul>
        <li><b>Songs:</b> Drum Show, Believer, The Search</li>
        <li><b>Activities:</b> reading, badminton, gaming, watching videos</li>
        <li><b>Animals:</b> Cheetah, peregrine falcon, ocean sunfish</li>
        <li><b>Plants:</b> Dragon tree, sequoia, bamboo, orchid</li>
        <li><b>Video Games:</b> Hollow Knight, The Witcher, Clair Obscur: Expedition 33, Hades</li>
    </ul>

    <!-- Numbered List -->
    <h2>Favorite Subjects (Ordered List)</h2>
    <ol>
        <li>Mobile System Programming for iOS</li>
        <li>Web Technologies and Web Design</li>
        <li>Software Requirements Analysis</li>
    </ol>

    <hr style="border-color: yellow;">

    <!-- Image Map -->
    <h2>Computer Image with Navigation Map</h2>

    <!-- Динамічний текст підказки -->
    <div id="status-text" class="status-box">Hover over any computer part (Monitor, Joystick, Disk Drive)...</div>

    <img src="computer.png" usemap="#compmap" class="comp-img" alt="Atari Computer">

<map name="compmap">
        <!-- Rectangle (rect): Monitor (зсунуто вліво на 1.5 см) -->
        <area shape="rect" coords="197,60,337,240" href="#monitor" alt="Monitor" 
              onmouseover="showText('🖥️ MONITOR: Displays color video image with Atari resolution.')" 
              onmouseout="hideText()">
        
        <!-- Polygon (poly): Disk Drive (зсунуто вліво на 1 см) -->
        <area shape="poly" coords="18,220,118,220,118,310,18,310" href="#diskdrive" alt="Disk Drive" 
              onmouseover="showText('💾 DISK DRIVE: Device for reading and writing floppy disks.')" 
              onmouseout="hideText()">
        
        <!-- Circle (circle): Joystick -->
        <area shape="circle" coords="555,250,45" href="#joystick" alt="Joystick" 
              onmouseover="showText('🕹️ JOYSTICK: Analog game controller with action button.')" 
              onmouseout="hideText()">
    </map>
    <div class="clear"></div>

    <!-- Anchor Descriptions -->
    <h2>Component Descriptions</h2>

    <div id="monitor">
        <h3>1. Monitor</h3>
        <p>The monitor displays a color video image with Atari system resolution.</p>
    </div>

    <div id="diskdrive">
        <h3>2. Disk Drive / System Unit</h3>
        <p>A device for reading and writing data on floppy disks.</p>
    </div>

    <div id="joystick">
        <h3>3. Joystick</h3>
        <p>An analog game controller with an action button for playing games.</p>
    </div>

    <!-- Скрипт виведення тексту -->
    <script>
        function showText(text) {
            const box = document.getElementById('status-text');
            box.innerText = text;
            box.classList.add('active');
        }

        function hideText() {
            const box = document.getElementById('status-text');
            box.innerText = "Hover over any computer part (Monitor, Joystick, Disk Drive)...";
            box.classList.remove('active');
        }
    </script>
</body>
</html>
