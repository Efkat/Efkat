```php
<?php

namespace App\Developer;

final class SymfonyDeveloper extends AbstractDeveloper
{
  use SymfonyTrait;
  use TwigTrait;
  
  public const FIRST_NAME = "Hugo";
  public const LAST_NAME = "Benabdelhak";
  
  public function __construct(
      \DateTimeImmutable $birthDate = new \DateTimeImmutable('2001-10-04T07:30:00'),
      string $currentCity = "Amiens",
      string $currentCompany = "No company"
  ){}
  
  public function getLinkedIn()
  {
    return new LinkedInPage("https://www.linkedin.com/in/hbenabdelhak/");
  }
}
```
