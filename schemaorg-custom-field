<?php
/**
 * Plugin Name: Schema.org Custom Field
 * Description: Adds a custom field named schema to the head-area.
 * Plugin URI:  https://github.com/gehwissenlos
 * Version:     0.1
 * Author:      Manuel Altherr
 * Author URI:  https://altherr.me/
 * Licence:     GPL 2
 * License URI: http://opensource.org/licenses/GPL-2.0
 */
defined( 'ABSPATH' ) or die( 'No script kiddies please!' );

function hook_schema_custom_field() {
  $schema = get_post_meta(get_the_ID(), 'schema', true);
  if(!empty($schema)) {
    echo $schema;
  }
}
add_action('wp_head', 'hook_schema_custom_field');
?>
