# flatten-js-browserified
flatten-js for browser

## installation


```sh

npm install cubic-spline-browserified

```

## usage

```html

<script src="node_modules/flatten-js-browserified/dist/flatten_js_browserified.js"></script>

<script>
    ...
        const point = new Point(100, 100);
        const vector = new Vector(1, 1);
        const circle = new Circle(point, 50);
        const line = new Line(new Point(50, 200), vector);
        const ray = new Ray(new Point(300, 300), vector);
        const segment = new Segment(new Point(400, 100), new Point(500, 200));
        const arc = new Arc(new Point(200, 300), 40, 0, Math.PI);
        const box = new Box(50, 50, 150, 150);
        const polygon = new Polygon();
        
        polygon.addFace([
            new Point(350, 50),
            new Point(450, 50),
            new Point(500, 150),
            new Point(400, 200),
            new Point(300, 150)
        ]);

        const matrix = new Matrix();
        matrix.translate(10, 20);

        const planarSet = new PlanarSet();
        planarSet.add(circle);
        planarSet.add(line);
        planarSet.add(segment);
    ...
</script>

```