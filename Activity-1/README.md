# Hackathon | Activity-1

### Problem statement
`print_iterative()` function should accept `$list` and print an html list.

Implement `print_iterative()` so that:

 - It traverses the array iteratively, not recursively.
 - It accounts for n depth (not just like the example list) where n is an integer.

See below example list:

```
<?php
$list = [
  'type' => 'ol',
  'items' => [
    [
      'text' => 'India',
      'child' => [
        'type' => 'ol',
        'items' => [
          [
            'text' => 'Maharashtra',
            'child' => [
              'type' => 'ul',
              'items' => [
                [
                  'text' => 'Pune',
                ],
                [
                  'text' => 'Nashik',
                ],
              ],
            ],
          ],
          [
            'text' => 'Karnataka',
          ],
          [
            'text' => 'Rajasthan',
            'child' => [
              'type' => 'ul',
              'items' => [
                [
                  'text' => 'Pushkar',
                ],
              ],
            ],
          ],
        ]
      ]
    ],
    [
      'text' => 'US',
      'child' => [
        'type' => 'ul',
        'items' => [
          [
            'text' => 'New York',
          ],
          [
            'text' => 'Kansas',
          ],
        ],
      ],
    ],
    [
      'text' => 'Pakistan',
      'child' => [
        'type' => 'ol',
        'items' => [
          [
            'text' => 'Balochistan',
          ],
          [
            'text' => 'Punjab',
            'child' => [
              'type' => 'ul',
              'items' => [
                [
                  'text' => 'Lahore',
                ],
                [
                  'text' => 'Faisalabad',
                ],
              ],
            ],
          ],
        ],
      ],
    ]
  ],
];
/**
 * Prints an html list iteratively.
 *
 * @param $list
 *
 * @return void
 */
function print_iterative($list) {
  // Code.
}
// Print list.
print_iterative($list);
```

#### Output
Example output:

```
<ul>
  <li>India
    <ul>
      <li>Maharashtra
        <ul>
          <li>Mumbai</li>
          <li>Pune</li>
        </ul>
      </li>
      <li>
        Rajasthan
      </li>
    </ul>
  </li>
  <li>
    Pakistan
    <ul>
      <li>
        Balochistan
        <ul>
          Lahore
        </ul>
      </li>
    </ul>
  </li>
</ul>
```
