<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">

    <title>Collapsible Tree Example</title>

    <style>

	.node circle {
	  fill: #fff;
	  stroke: steelblue;
	  stroke-width: 3px;
	}

	.node text { font: 12px sans-serif; }

	.link {
	  fill: none;
	  stroke: #ccc;
	  stroke-width: 2px;
	}

    </style>

  </head>

  <body>

<!-- load the d3.js library -->
<script src="https://d3js.org/d3.v3.min.js"></script>

<script>

var json =
{
    "name": "Base",
    "children": [
        {
            "name": "Type A",
            "children": [
                {
                    "name": "Section 1",
                    "children": [
                        {"name": "Child 1"},
                        {"name": "Child 2"},
                        {"name": "Child 3"}
                    ]
                },
                {
                    "name": "Section 2",
                    "children": [
                        {"name": "Child 1"},
                        {"name": "Child 2"},
                        {"name": "Child 3"}
                    ]
                }
            ]
        },
        {
            "name": "Type A",
            "children": [
                {
                    "name": "Section 1",
                    "children": [
                        {"name": "Child 1"},
                        {"name": "Child 2"},
                        {"name": "Child 3"}
                    ]
                }
            ]
        }
    ]
};
// ************** Generate the tree diagram	 *****************
var margin = {top: 40, right: 120, bottom: 20, left: 120},
	width = 1100 - margin.right - margin.left,
	height = 1100 - margin.top - margin.bottom,
  i = 0;

var tree = d3.layout.tree().size([height, width]);

var diagonal = d3.svg.diagonal()
	.projection(function(d) { return [d.x, d.y]; });

var svg = d3.select("body").append("svg")
	.attr("width", width + margin.right + margin.left)
	.attr("height", height + margin.top + margin.bottom)
  .append("g")
	.attr("transform", "translate(" + margin.left + "," + margin.top + ")");

root = json;

update(root);

function update(source) {

  // Compute the new tree layout.
  var nodes = tree.nodes(root).reverse(),
	  links = tree.links(nodes);

  // Normalize for fixed-depth.
  nodes.forEach(function(d) { d.y = d.depth * 100; });

  // Declare the nodes…
  var node = svg.selectAll("g.node")
	  .data(nodes, function(d) { return d.id || (d.id = ++i); });

  // Enter the nodes.
  var nodeEnter = node.enter().append("g")
	  .attr("class", "node")
	  .attr("transform", function(d) {
		  return "translate(" + d.x + "," + d.y + ")"; });

  nodeEnter.append("rect")
	  // .attr("r", 10)
    .attr("x", -10)
    .attr("y", -10)
    .attr("width", 150)
    .attr("height", 50)
	  .style("fill", "lightblue")
    .style("opacity", "0.5");

  nodeEnter.append("text")
	  .attr("y", function(d) {
		  return d.children || d._children ? -18 : 18; })
	  .attr("dy", ".35em")
	  .attr("text-anchor", "middle")
	  .text(function(d) { return d.name; })
	  .style("fill-opacity", 1);

  // Declare the links…
  var link = svg.selectAll("path.link")
	  .data(links, function(d) { return d.target.id; });

  // Enter the links.
  link.enter().insert("path", "g")
	  .attr("class", "link")
	  .attr("d", diagonal);

}

</script>

  </body>
</html>
