DayZ Chernarus New 1.26 Sakhal / Frostline Item Class Names In Types README & Terms Of Use

------------------------------------------

Limited Testing on PC Chernarus Local Server DAYZ EXPERIMENTAL Version 1.26 AUG 2024.

Created by @scalespeeder. Please report bugs & errors to scalespeeder@gmail.com with screenshots.

TERMS OF USE
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded xml files could break the functioning of your DAYZ server, requiring a reinstall that would wipe
all player progress.

Using these modded xml files neccessitates increased regular restarts to prevent server crashing.

It is suggested you thoroughly test your server after applying these files to ensure proper
functioning of your server.

-----------------------------------------

These are the new class-names that have been added to the DayZ types.xml server file in experimental update 1.26, in the Chernarus types file.

I have inlcuded two files, one which has just the new entries copied from the 1.26 files, and the other in spawnable format where I have edited nominals, mins, useages, etc so the file can
either be added to your custom 1.25 types when 1.26 goes live, so these items will spawn, or you can use cfgeconomycore to refore to the file,
 see https://community.bistudio.com/wiki/DayZ:Central_Economy_mission_files_modding for advice, remember on console any extra mission files MUST be in the "custom" directory.
 
THESE CLASS NAMES WILL ONLY WORK ON EXPERIMENTAL 1.26 SERVERS OR WHEN 1.26 GOES LIVE TO PUBLIC SERVERS!

WE'RE GETTING BOATS TOO ON THIS UPDATE - I'VE INCLUDED THEM TOO, BUT REMEMBER THESE WILL BE SPAWNED BY NEW ENTRIES IN EVENTS.XML & CFGEVENTSPAWNS.XML, WITH AN ENTRY IN CFGSPAWNABLESTYPES.XML SO LEAVE TYPES.XML NOMINALS AT ZERO.

I HAVE INCLUDED THE EVENTS.XML , CFG SPAWABLETYPES.XML & CFGEVENTSPAWNS.XML BOAT SNIPPETS BELOW:

<!--ADD THIS TO CHERNARUS EVENTS.XML -->

 <event name="VehicleBoat">
        <nominal>22</nominal>
        <min>18</min>
        <max>24</max>
        <lifetime>600</lifetime>
        <restock>0</restock>
        <saferadius>500</saferadius>
        <distanceradius>500</distanceradius>
        <cleanupradius>200</cleanupradius>
        <flags deletable="0" init_random="0" remove_damaged="1"/>
        <position>fixed</position>
        <limit>mixed</limit>
        <active>1</active>
        <children>
            <child lootmax="0" lootmin="0" max="10" min="6" type="Boat_01_Black"/>
            <child lootmax="0" lootmin="0" max="10" min="6" type="Boat_01_Blue"/>
            <child lootmax="0" lootmin="0" max="0" min="0" type="Boat_01_Camo"/>
            <child lootmax="0" lootmin="0" max="10" min="6" type="Boat_01_Orange"/>
        </children>
    </event>
	
<!--OR ADD THIS TO LIVONIA EVENTS.XML -->

<event name="VehicleBoat">
        <nominal>5</nominal>
        <min>2</min>
        <max>6</max>
        <lifetime>6000</lifetime>
        <restock>0</restock>
        <saferadius>500</saferadius>
        <distanceradius>500</distanceradius>
        <cleanupradius>200</cleanupradius>
        <flags deletable="0" init_random="0" remove_damaged="1"/>
        <position>fixed</position>
        <limit>mixed</limit>
        <active>1</active>
        <children>
            <child lootmax="0" lootmin="0" max="10" min="5" type="Boat_01_Black"/>
            <child lootmax="0" lootmin="0" max="10" min="5" type="Boat_01_Blue"/>
            <child lootmax="0" lootmin="0" max="10" min="5" type="Boat_01_Orange"/>
        </children>
    </event>
	
<!-- ADD THIS TO CHERNARUS AND OR LIVONIA CFGSPAWNABLETYPES.XML -->

<type name="Boat_01_Black">
		<attachments chance="0.20">
			<item name="SparkPlug" chance="1.0" />
		</attachments>
	</type>
	<type name="Boat_01_Blue">
		<attachments chance="0.20">
			<item name="SparkPlug" chance="1.0" />
		</attachments>
	</type>
	<type name="Boat_01_Camo">
		<attachments chance="0.20">
			<item name="SparkPlug" chance="1.0" />
		</attachments>
	</type>
	<type name="Boat_01_Orange">
		<attachments chance="0.20">
			<item name="SparkPlug" chance="1.0" />
		</attachments>
	</type>
	
<!-- ADD THIS TO CHERNARUS CFGEVENTSPAWNS.XML-->

<event name="VehicleBoat">
		<pos x="1716.188110" z="2000.763306" />
		<pos x="1748.611328" z="2014.182007" />
		<pos x="2333.722656" z="1982.005127" />
		<pos x="2347.214600" z="1973.808472" />
		<pos x="2933.019775" z="1941.380615" />
		<pos x="2950.001953" z="1943.084961" />
		<pos x="3580.907471" z="2107.369385" />
		<pos x="3642.509277" z="2109.567871" />
		<pos x="4087.289307" z="2193.691650" />
		<pos x="4098.899414" z="2186.442871" />
		<pos x="4313.916504" z="2253.489258" />
		<pos x="4403.475586" z="2205.808105" />
		<pos x="5879.444336" z="1963.862183" />
		<pos x="6157.993652" z="2053.256348" />
		<pos x="6160.095215" z="2011.115723" />
		<pos x="6219.329102" z="2018.734863" />
		<pos x="6313.021484" z="2195.519775" />
		<pos x="6445.172852" z="2164.079834" />
		<pos x="6549.093262" z="2250.669189" />
		<pos x="6569.554688" z="2250.365479" />
		<pos x="7035.903809" z="2460.037598" />
		<pos x="7295.582520" z="2659.069580" />
		<pos x="7415.538086" z="2560.321289" />
		<pos x="7811.205078" z="2760.277832" />
		<pos x="8080.232910" z="2742.809570" />
		<pos x="8198.986328" z="2755.958252" />
		<pos x="8267.049805" z="2461.652588" />
		<pos x="8305.828125" z="2592.269287" />
		<pos x="8333.263672" z="2366.555664" />
		<pos x="8475.794922" z="2426.969238" />
		<pos x="8802.299805" z="2154.909912" />
		<pos x="8858.551758" z="2082.438721" />
		<pos x="9343.027344" z="1844.759277" />
		<pos x="9783.181641" z="1764.526733" />
		<pos x="9783.534180" z="1747.436401" />
		<pos x="9954.826172" z="1751.823486" />
		<pos x="9957.985352" z="1604.198364" />
		<pos x="10059.670898" z="1597.689697" />
		<pos x="10229.332031" z="1561.574585" />
		<pos x="10421.437500" z="1734.374512" />
		<pos x="10468.315430" z="1833.428223" />
		<pos x="10698.851563" z="2123.040527" />
		<pos x="10881.899414" z="2336.180420" />
		<pos x="10952.043945" z="2632.239746" />
		<pos x="11077.573242" z="2666.339355" />
		<pos x="12037.817383" z="3398.442871" />
		<pos x="12158.946289" z="3404.761719" />
		<pos x="12378.870117" z="3437.083496" />
		<pos x="12945.443359" z="8919.328125" />
		<pos x="12989.865234" z="3651.347656" />
		<pos x="13046.505859" z="8468.286133" />
		<pos x="13053.779297" z="9485.443359" />
		<pos x="13081.017578" z="9893.432617" />
		<pos x="13085.416016" z="8205.884766" />
		<pos x="13102.666016" z="9694.800781" />
		<pos x="13102.693359" z="3721.000244" />
		<pos x="13137.059570" z="7813.878418" />
		<pos x="13262.733398" z="3753.452148" />
		<pos x="13268.749023" z="7286.617676" />
		<pos x="13272.000977" z="10128.308594" />
		<pos x="13332.088867" z="7083.145996" />
		<pos x="13359.411133" z="10709.581055" />
		<pos x="13462.985352" z="5446.159668" />
		<pos x="13528.787109" z="6418.449219" />
		<pos x="13549.652344" z="6247.452148" />
		<pos x="13554.335938" z="3839.198730" />
		<pos x="13605.369141" z="4432.208496" />
		<pos x="14393.814453" z="13210.004883" />
		<pos x="14434.454102" z="13260.297852" />
		<pos x="15211.263672" z="13814.097656" />
		<pos x="15227.822266" z="13816.418945" />
		<pos x="15244.462891" z="13821.070313" />
	</event>
	
	<!-- ADD THIS TO LIVONIA CFGEVENTSPAWNS.XML-->
	
		<event name="VehicleBoat">
		<pos x="736.904724" z="7630.322754" />
		<pos x="1211.179443" z="7596.854004" />
		<pos x="2558.610352" z="8138.580078" />
		<pos x="3245.947510" z="8946.619141" />
		<pos x="3636.865234" z="9095.704102" />
		<pos x="4125.540039" z="8968.368164" />
		<pos x="5285.077148" z="9487.263672" />
		<pos x="5507.043457" z="9890.708008" />
		<pos x="5758.463867" z="10178.937500" />
		<pos x="6231.461914" z="10768.079102" />
		<pos x="6378.429688" z="10766.851563" />
		<pos x="6421.747559" z="10888.140625" />
		<pos x="7926.263184" z="11878.577148" />
		<pos x="8425.622070" z="11874.351563" />
		<pos x="9516.850586" z="11719.943359" />
		<pos x="11239.161133" z="11245.859375" />
		<pos x="11794.729492" z="10940.535156" />
	</event>

Thanks, Rob.

