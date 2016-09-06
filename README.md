# RTLit

RTLit is a set of mixins which let you make any CSS Framework RTL. Using predefined bidirectional mixins you will be able to replace simple css commands with a mixin which can detect the direction and generate bidirectional commands.

# Current Version

## 3.0

Old versions
### 2.0 => SCSS support
### 1.0 => LESS support

Ask your question on twitter via [@hadjloo](http://twitter.com/hadjloo)

# Team

## Nasser Hadjloo
Project owner.
[n.hajloo@gmail.com](mailto:n.hajloo@gmail.com)

#Documentation

in your main file *include RTLit* file (RTLit.less or RTLit.scss or RTLit.styl)

instead of standard css commands use RTLit mixins such as

## LESS

padding: 4px 0 15px 12px;               => .SwapPadding(4px, 0, 15px, 12px);

left: 50px;                             => .DockItem("left", 50px);

text-align: left !important;            => .TextAlignTo("left") !important;

margin-left: 32px;                      => .MarginLeftOrRight("margin-left", 32px);

border-right: 3px blue solid            => .BorderLeftOrRight("border-right", 3px, blue, solid);


## SCSS

padding: 4px 0 15px 12px;               => @include SwapPadding(4px, 0, 15px, 12px);

left: 50px;                             => @include DockItem("left", 50px);

text-align: left !important;            => @include TextAlignTo("left", $important: true);

margin-left: 32px;                      => @include MarginLeftOrRight("margin-left", 32px);

border-right: 3px blue solid            => @include BorderLeftOrRight("border-right", 3px, blue, solid);


## STYLUS lang

padding: 4px 0 15px 12px;               => SwapPadding(4px, 0, 15px, 12px);

left: 50px;                             => DockItem("left", 50px);

text-align: left !important;            => TextAlignTo("left", $important = true);

margin-left: 32px;                      => MarginLeftOrRight("margin-left", 32px);

border-right: 3px blue solid            => BorderLeftOrRight("border-right", 3px, blue, solid);


# Pull requests

Please create pull requests for develop branch.
