# ion-img

Img is a tag that will lazily load an image when ever the tag is in the viewport. This is extremely useful when generating a large list as images are only loaded when they're visible. The component uses [Intersection Observer](https://caniuse.com/#feat=intersectionobserver) internally, which is supported in most modern browser, but falls back to a `setTimeout` when it is not supported.


<!-- Auto Generated Below -->


## Usage

### Angular

```html
<ion-list>
  <ion-item *ngFor="let item of items">
    <ion-thumbnail slot="start">
      <ion-img [src]="item.src"></ion-img>
    </ion-thumbnail>
    <ion-label>{{item.text}}</ion-label>
  </ion-item>
</ion-list>
```



## Properties

| Property | Attribute | Description                                                                                                                                                                                                              | Type                  | Default     |
| -------- | --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------- | ----------- |
| `alt`    | `alt`     | This attribute defines the alternative text describing the image. Users will see this text displayed if the image URL is wrong, the image is not in one of the supported formats, or if the image is not yet downloaded. | `string \| undefined` | `undefined` |
| `src`    | `src`     | The image URL. This attribute is mandatory for the <img> element.                                                                                                                                                        | `string \| undefined` | `undefined` |


## Events

| Event           | Description                        | Detail |
| --------------- | ---------------------------------- | ------ |
| `ionImgDidLoad` | Emitted when the img src is loaded | void   |


----------------------------------------------

*Built with [StencilJS](https://stenciljs.com/)*
