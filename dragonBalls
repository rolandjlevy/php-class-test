<html>
  <head>
    <title>DragonBalls Test</title>
  </head>
  <body>
    <?php

    class DragonBalls {
      // Properties
      public $max;
      public $question;
      public $group = [];

      // Methods
      function set_question($question) {
        $this->question = $question;
      }
      function set_max($max) {
        $this->max = $max;
      }
      function ask_question() {
        if (count($this->group) == $this->get_max()) {
          echo 'All ' . $this->get_max() . ' Dragon Balls found, so ' . $this->question;
        }
      }
      function get_max() {
        return $this->max;
      }
      function init_group() {
        for ($i = 0; $i < $this->get_max(); $i++) {
          $this->group[] = array('id' => ($i+1), 'name' => 'Dragon Ball ' . ($i+1));
        }
      }
      function search_group() {
        echo '<h3>Search all Dragon Balls</h3>';
        echo '<pre>';
        foreach ($this->group as $key => $value) {
          print_r($value);
        }
        echo '</pre>';
      }
    }

    $allDragonBalls = new DragonBalls();
    $allDragonBalls->set_max(7);
    $allDragonBalls->set_question('what do you want?');
    $allDragonBalls->init_group();
    $allDragonBalls->search_group();
    $allDragonBalls->ask_question();

  ?>

  </body>
</html>
