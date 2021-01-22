---
id: dxGantt.Options.onTaskClick
type: function(e)
default: null
EventForAction: dxGantt.taskClick
---
---
##### shortDescription
A function that is executed when a user clicks a task.

##### param(e): Object
Information about the event.

##### field(e.component): {WidgetName}
The UI component's instance.

##### field(e.data): any
The task data.

##### field(e.element): dxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.event): event
#include common-ref-eventparam

##### field(e.key): any
The task key.

##### field(e.model): Object
Model data. Available only if you use Knockout.

---

---

##### jQuery

    <!-- tab: index.js -->
    $(function() {
        $("#gantt").dxGantt({
            // ...
            onTaskClick: function (e) {
                if (e.key != 0) {
                    // your code
                }
            }
        });
    }); 

---

#####See Also#####
- [taskClick](/Documentation/ApiReference/UI_Components/dxGantt/Events/#taskClick)
- [Gantt Elements](/Documentation/Guide/UI_Components/Gantt/Gantt_Elements/)