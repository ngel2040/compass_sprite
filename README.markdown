# compass sprite

## example

    @include sprite("sprites/*.png", "sprite");

    @include retina_sprite("sprites_x2/*.png", "sprite_x2");

Merges images in the image folder

retina support


image folder

filename1.png, filename2.png

scss

    @include sprite("sprites/*.png", "sprite");

css

    .sprite, .filename1, .filename2 {
      display: inline-block;
      position: relative;
      overflow: hidden;
      background-image: url('../images/sprites-sff15fd9ddd.png');
      background-repeat: no-repeat;
    }
    .sprite span, .filename1 span, .filename2 span {
      display: inline-block;
      text-indent: -9999em;
      outline: 0;
    }
    .filename1 {
      width: 30px;
      height: 30px;
      background-position: 0 0;
    }
    .filename2 {
      width: 194px;
      height: 54px;
      background-position: 0 -30px;
    }
