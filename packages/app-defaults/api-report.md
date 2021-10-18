## API Report File for "@backstage/app-defaults"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import { AppComponents } from '@backstage/core-app-api';
import { AppIcons } from '@backstage/core-app-api';
import { AppOptions } from '@backstage/core-app-api';
import { AppTheme } from '@backstage/core-plugin-api';
import { BackstageApp } from '@backstage/core-app-api';
import { IconComponent } from '@backstage/core-plugin-api';

// @public
export function createApp(
  options?: Omit<AppOptions, keyof OptionalAppOptions> & OptionalAppOptions,
): BackstageApp;

// @public
export type OptionalAppOptions = {
  icons?: Partial<AppIcons> & {
    [key in string]: IconComponent;
  };
  themes?: (Partial<AppTheme> & Omit<AppTheme, 'theme'>)[];
  components?: Partial<AppComponents>;
};
```