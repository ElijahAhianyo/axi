# Axi Planner

[_Documentation generated by Documatic_](https://www.documatic.com)

<!---Documatic-section-Codebase Structure-start--->
## Codebase Structure

<!---Documatic-block-system_architecture-start--->
```mermaid
None
```
<!---Documatic-block-system_architecture-end--->

# #
<!---Documatic-section-Codebase Structure-end--->

<!---Documatic-section-axi.planner.Planner-start--->
## [axi.planner.Planner](10-axi_planner.md#axi.planner.Planner)

<!---Documatic-section-Planner-start--->
<!---Documatic-block-axi.planner.Planner-start--->
<details>
	<summary><code>axi.planner.Planner</code> code snippet</summary>

```python
class Planner(object):

    def __init__(self, acceleration, max_velocity, corner_factor):
        self.acceleration = acceleration
        self.max_velocity = max_velocity
        self.corner_factor = corner_factor

    def plan(self, points):
        return constant_acceleration_plan(points, self.acceleration, self.max_velocity, self.corner_factor)

    def plan_all(self, paths):
        return [self.plan(path) for path in paths]
```
</details>
<!---Documatic-block-axi.planner.Planner-end--->
<!---Documatic-section-Planner-end--->

# #
<!---Documatic-section-axi.planner.Planner-end--->

[_Documentation generated by Documatic_](https://www.documatic.com)