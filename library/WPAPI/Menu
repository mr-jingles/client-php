
<?php
/**
 * Menu entity object
 *
 * @package WordPress API Client
 * @subpackage Entities
 */
/**
 * Menu entity object
 *
 * @package WordPress API Client
 * @subpackage Entities
 */
class WPAPI_Menu {
	/**
	 * Data container
	 *
	 * @var array
	 */
	protected $data;
	/**
	 * Keys that have been changed since last update
	 *
	 * @var array
	 */
	protected $changed = array();
	
	/**
	 * Get a property
	 *
	 * See the specification for data keys/values returned by the API.
	 *
	 * @param string $key Key to retrieve
	 * @return mixed Menu value for the key
	 */
	public function __get($key) {
		if (!isset($this->data[$key])) {
			return null;
		}
		return $this->data[$key];
	}
	/**
	 * Set a property
	 *
	 * @param string $key Key to replace
	 * @param mixed $value Value for the key
	 */
	public function __set($key, $value) {
		$this->data[$key] = $value;
		$this->changed[$key] = true;
	}
	/**
	 * Get the raw internal Menu data
	 *
	 * Avoid use in favour of accessing via the properties instead.
	 *
	 * @return array Raw data from the API
	 */
	public function getRawData() {
		return $this->data;
	}
	
}
