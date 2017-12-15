# hello-world

// change check box color
event.target.fillColor = event.target.value=="Off" ? color.white : color.gray;


//Radio color
function processCBGroup(doc, ev)
{
    var fYes = doc.getField(ev.target.name + ".0");

 

    var fNo = doc.getField(ev.target.name + ".1");

 

    var fUnsure = doc.getField(ev.target.name + ".2");

 

    (ev.target.value == "Yes") ? fYes.fillColor = color.green : fYes.fillColor = color.transparent;

 

    (ev.target.value == "No") ? fNo.fillColor = color.red : fNo.fillColor = color.transparent;

 

    (ev.target.value == "Unsure") ? fUnsure.fillColor = color.yellow : fUnsure.fillColor = color.transparent;


}