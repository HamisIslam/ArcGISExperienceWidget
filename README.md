# Add-Remove Feature Service

This widget demonstrates how to add feature service layers to a mab .



## How it works

Within `widget.tsx`, in the `render()` function, the url is inserted to a text-input by the user and get added by add button  and can be removed by remove button :



The `onChange` handler is setup to call the `getData` function when the user insert feature service url.

A reference to the Map object is acquired using the `JimuMapViewComponent` module.

```js
// Create and add the new Feature Layer
const featureLayer = new FeatureLayer({
  url: url,
});
this.state.jimuMapView.view.map.add(featureLayer);
```
