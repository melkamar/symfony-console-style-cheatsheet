# Symfony Console Style cheatsheet

Reference for how the [Style component](https://symfony.com/doc/current/console/style.html) actually looks like.

<img width="859" alt="image" src="https://github.com/user-attachments/assets/96e3ef7f-f88f-4973-86b4-858b0ab55372" />

## Code

```php
    protected function execute(InputInterface $input, OutputInterface $output) : int
    {
        $this->io->title('Title');
        $this->io->section('Section');

        $this->io->text(['Text', 'Text']);
        $this->io->listing(['Listing', 'Listing']);
        $this->io->definitionList('definitionList title', ['A' => 'Text', 'B' => 'Text']);

        $this->io->note(['Note', 'Note']);
        $this->io->caution(['Caution', 'Caution']);

        $this->io->success(['Success', 'Success']);
        $this->io->info(['Info', 'Info']);
        $this->io->warning(['Warning', 'Warning']);
        $this->io->error(['Error', 'Error']);

        return 0;
    }
```
