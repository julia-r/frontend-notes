# Responsive Images

## Serving different assets with media queries

Sometimes you have big background images fpr websites,
because the design should look good on big screens. So background-images with a width of 2000px
are not rare. But what if a user with a tablet or a mobile phone visits that site?
He wont't see the whole image anyway, so we can send him a smaller one.

You can use Media queries to show different assets for background images,
depending on the viewport width.

*Example:*
```css
body {
    background-image: url('img/background.jpg');
}

@media screen and (max-width: 1024px) {
	body {
		background-image: url('img/background-1024.jpg');
	}
}

@media screen and (max-width: 720px) {
	body {
		background-image: url('img/background-720.jpg');
	}
}
```

This works well for background images, where we usually do not care if a bit of
the sides is cut off or not. It is mostly decoration.

## Responsive Inline Images

Keep their width height ratio.

## Responsive Background Images

Do not keep their width height ratio, we need to use a trick here.

http://inspectelement.com/tutorials/a-responsive-css-background-image-technique/

## Responsive Image Sprites

http://blog.brianjohnsondesign.com/responsive-background-image-sprites-css-tutorial/
