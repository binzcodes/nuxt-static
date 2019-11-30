<template>
  <div class="rbinzLogo">
    <div class="Triangle Triangle--two" />
    <div class="Triangle Triangle--two--lighten" />
    <div class="Triangle Triangle--one" />
    <div class="Triangle Triangle--one--lighten" />
    <div class="Triangle Triangle--three" />
    <div class="Triangle Triangle--three--lighten" />
    <div class="Triangle Triangle--four" />
  </div>
</template>

<style>
.rbinzLogo {
  display: inline-block;
  position: relative;
  overflow: hidden;
  height: 180px;
  width: 245px;
}

.Triangle {
  position: absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 0;
}

.Triangle--one {
  border-left: 105px solid transparent;
  border-right: 105px solid transparent;
  border-top: 180px solid #83e0a4;
}

.Triangle--one--lighten {
  border-left: 105px solid transparent;
  border-top: 180px solid #98eab5;
}

.Triangle--two {
  left: 70px;
  border-left: 87.5px solid transparent;
  border-right: 87.5px solid transparent;
  border-top: 150px solid #43a1c5;
}

.Triangle--two--lighten {
  left: 70px;
  border-left: 87.5px solid transparent;
  border-top: 150px solid #7dc6e1;
}

.Triangle--three {
  left: 70px;
  border-left: 70px solid transparent;
  border-right: 70px solid transparent;
  border-top: 120px solid #184757;
}

.Triangle--three--lighten {
  left: 70px;
  animation: gorightTwoHighlight 0.5s linear forwards 3.5s;
  border-left: 70px solid transparent;
  border-top: 120px solid #23596b;
}
</style>
