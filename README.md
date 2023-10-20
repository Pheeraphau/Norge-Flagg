# Norge-Flagg
white-rectangle = rectangle(22 * 15, 16 * 15, "solid", "white")
red-left-rectangle = square(6 * 15, "solid", "crimson")
red-right-rectangle = rectangle(12 * 15, 6 * 15, "solid", "crimson")
blue-vertical = rectangle(2 * 15, 16 * 15, "solid", "navy")
blue-horizontal = rectangle(22 * 15, 2 * 15, "solid", "navy")

top-left = overlay-align("left", "top", red-left-rectangle, white-rectangle)
bottom-left = overlay-align("left", "bottom", red-left-rectangle,(top-left))
top-right = overlay-align("right", "top", red-right-rectangle,(bottom-left))
bottom-right = overlay-align("right", "bottom", red-right-rectangle, (top-right))
vertical-line = overlay-xy(blue-vertical,-106,0,(bottom-right))
final-flag = overlay-xy(blue-horizontal,0,-106,(vertical-line))