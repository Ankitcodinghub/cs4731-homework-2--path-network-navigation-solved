# cs4731-homework-2--path-network-navigation-solved
**TO GET THIS SOLUTION VISIT:** [CS4731 Homework 2- Path Network Navigation Solved](https://www.ankitcodinghub.com/product/cs4731-homework-2-path-network-navigation-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;123268&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS4731 Homework 2- Path Network Navigation Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Make sure you first watch the Path Network lecture before attempting this assignment.

One of the main uses of artificial intelligence in games is to perform <em>path planning</em>, the search for a sequence of movements through the virtual environment that gets an agent from one location to another without running into any obstacles. For now, we will assume static obstacles. In order for an agent to engage in path planning, there must be a topography for the agent to traverse that is represented in a form that can be efficiently reasoned about.

Grid topologies discretize the environment and usually assumes an agent can be in one discrete cell or another. However, for many games such as 1st-person shooters, a more continuous model of space is beneficial. Depending on the granularity of the grid, a lot of space around obstacles becomes inaccessible in grid-based approaches. Finally, grids result in unnecessarily large number of cell transitions.

&nbsp;

A <strong>path network</strong> is a set of path nodes and edges that facilitates obstacle avoidance. The path network discretizes a continuous space into a small number of points and edges that allow transitions between points. However, unlike a grid topology, a path network does not require the agent to be at one of the path nodes at all times. The agent can be at any point in the terrain. When the agent needs to move to a different location and an obstacle is in the way, the agent can move to the nearest path node accessible by straight-line movement and then find a path through the edges of the path network to another path node near to the desired destination.

&nbsp;

In this assignment, you will be provided with different terrains with obstacles and hard-coded path nodes. You must write the code to generate the path network, as a set of edges between path nodes. An edge between path nodes exists when (a) there is no obstacle or boundary wall between the two path nodes, (b) there is sufficient space on either side of the edge so that an agent can follow the line without colliding with any obstacles or boundary wall and (c) a path node that is inside the boundary but outside of any obstacles. Nodes that are outside of the boundary or inside of obstacles, should not connect.

&nbsp;

Furthermore, there should be edges in both directions. If there is an edge from Node A to Node B, then there should be an edge from Node B to Node A. Also, if there should be an edge from Node A to Node B, it should appear exactly once in the edge list for Node A (no duplicates). Also, no nodes should link to self.

&nbsp;

If two nodes are arbitrarily close together, including possibly located at exactly the same location, they should still be connected.

&nbsp;

<h1>What you need to know</h1>
Please consult <strong>homework 1</strong> for background on the Unity Project. In addition to the information about the game engine provided there, the following applies.

&nbsp;

Also, make sure you first watch the Path Network lecture before attempting this assignment.

&nbsp;

<h2>CreatePathNetwork</h2>
This is the only file you will be modifying and submitting for this homework. It provided functionality to create a path network from provided pathNodes.

&nbsp;

String StudentAuthorName – Please change to your name

&nbsp;

<em>Create() </em>

&nbsp;

This is the method you will be finishing. You can create helper methods in the same source code file if you like.

&nbsp;

Parameters:

Vector2 canvasOrigin – Bottom left corner of navigable space float canvasWidth – Width of navigable space float canvasHeight – Height of navigable space

List&lt;Polygon&gt; obstacles – The polygon obstacles that obstruct candidate pathEdges between nodes. Furthermore, end points cannot be within agentRadius distance (less-than test) of a candidate pathEdges

float agentRadius – The radius of the agent (don’t expect to always be the same).

The agentRadius will always be greater than zero

float minPoVDist – The minimum distance a single point of visibility can be from the vertex or lines of angle that is bisected. Only used when generating PoVs

float maxPoVDist – The maximum distance a single point of visibility can be from the

vertex or lines of angle that is bisected. Only used when generating PoVs

ref List&lt;Vector2&gt; pathNodes – The nodes of the graph. You use them as provided if mode is PathNetworkMode.Predefined. But you generate them if mode is PathNetworkMode.PointsOfVisibility

out List&lt;List&lt;int&gt;&gt; pathEdges – A list of valid edges, indexing the pathNodes. This is generated by your code. All valid edges should be generated. pathEdges will be returned empty if there are no nodes to consider.

PathNetworkMode mode – enum that is either PathNetworkMode.Predefined. or PathNetworkMode.PointsOfVisibility. The first specifies that path nodes are provided to Create() for connection. The second specifies that path nodes must be generated according to PoV algorithm.

<strong>&nbsp;</strong>

<h2>PathNetwork</h2>
The PathNetwork calls your CreatePathNetwork.Create() to generate the path network and also performs visualization and other related tasks. You don’t need to modify anything in this file, but may find it useful to see how your code is called.

&nbsp;

<h2>PathNetworkTest</h2>
This file is for unit/integration testing. You are highly encouraged to create your own tests.

For instance, you might consider different numbers of nodes present, including edge cases. Passing the provided example test(s) in this file does NOT indicate that you have a correct solution!

<h2>Miscellaneous utility functions</h2>
Methods you need for this assignment are provided at the top of CreatePathNetwork.cs

Also, you will access Polygon member methods such as getIntegerPoints() and getPoints()

&nbsp;

In terms of Computational Geometry, the DistanceToLineSegment() works best with floats. You can use the poly.getPoints(), which are unscaled floats. The poly.getIntegerPoints() are the equivalent vectors in scaled integer form (by 1000).

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;</strong>

<h1>Instructions</h1>
To complete this assignment, you must (1) implement code to generate a path network for a set of given path nodes in a given scene. The path network should guarantee that an agent will not collide with an obstacle between any starting point and any destination point in the world.

&nbsp;

It is not required, nor graded, but you can consider implementing Points of Visibility support as well. See below for details.

&nbsp;

To run the project code, use the following commands:

&gt;<strong> Step 1:</strong> Download the project from github. Open the project in Unity. Open scene PathNetwork

&gt;<strong> Step 2:</strong> If you hit play, you should see a list of path nodes and some obstacles not connected to each other. You can click the obstacles and path nodes to drag them around.

You can press buttons 1,2,3,… to test some preconfigured obstacle/pathNode positions.

Clicking outside of an obstacle initiates path planning. Spacebar changes search strategies.

Note that any search that relies on AStar won’t function until you implement it. <strong>&gt; Step 3:</strong> Create the edges in the path network.

Open Assets/Scripts/GameAIStudentWork/PathNetwork/CreatePathNetwork.cs. Update the name string first! Implement the functionality to generate a valid list of PathEdges connecting PathNodes that are not obstructed from each other. Also, obstacles cannot be too close to PathEdges for the agent to fit by while following an edge.

<strong>&nbsp;</strong>

&nbsp;

&nbsp;

&nbsp;

&nbsp;

<h1>Grading</h1>
We will grade your solution based on the following criterion:

<ul>
<li><strong>Reachability: </strong>The path network should be such that an agent can navigate from any path node to any other path node along any edge in the network without colliding with an obstacle or canvas/world boundary. No edges that are out of bounds (outside boundary or inside obstacles).</li>
<li><strong>Graph Characteristics: </strong>Valid edges should have a corresponding edge going opposite direction between same two nodes. There should be no duplicate edges in each edge list. Nodes should not have an edge directly back to itself. Edge lists should never be null (empty is allowed). Edge lists should not reference non existent node indexes. PathNodes and pathEdges should be the same length.</li>
<li><strong>Points of Visibility:</strong> You don’t need to respond to the PathNetworkMode mode parameter. But you can optionally implement Points of Visibility support.</li>
</ul>
Please remove all print statements before submitting. The autograder will only provide a few hundred lines of feedback and you might overflow the buffer so that the informative part doesn’t show up. Also, print statements can cause significant slowdown such that you might fail a test due to timeout (see below). When you remove print statements, please test your code again! Quite often we receive assignments that don’t compile due to a hanging <em>ifstatement</em> where a print() was the consequent.

&nbsp;

Your code will be allowed at least 10 seconds to complete each test.

&nbsp;

&nbsp;

<h1>Hints</h1>
Make sure any edge in the path network is traversable by an agent that has physical size. That is, edges in the path network should never come too close to any Obstacle such that an agent blindly following the path edge collides with an Obstacle (or the edges of the map). It doesn’t matter how close two path nodes are to one another. If an agent can be centered at one node and traverse in a straight line (without intersecting any obstacles) to another node then the two nodes should be connected by an edge.

&nbsp;

Create additional presets by adding more configurations to Assets/Scripts/Config/CustomPresetConfig.cs However, you do not submit this file.

&nbsp;

Also, create Unit/Integration tests with PathNetworkTest.cs (also do not submit).

&nbsp;

<h1>Submission</h1>
To submit your solution, upload your modified CreatePathNetwork.cs with your name properly set in the name string. All work should be done within this file.

&nbsp;

You should not modify any other files in the game engine (other than optionally CustomPresetConfig.cs for your own testing purposes).

&nbsp;

DO NOT upload the entire game engine.

&nbsp;

Refer to Canvas assignment description for submission instructions (probably GradeScope).

&nbsp;

&nbsp;

<h2>Advanced Method</h2>
<strong>&nbsp;</strong>

Not required (or graded), but you might optionally try to implement Points of Visibility if the mode parameter is set to PointsOfVisibility. Refer to lecture for the details of the Points of Visibility method of node placement.

&nbsp;
