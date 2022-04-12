## API Report File for "@backstage/plugin-search-react"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import { ApiRef } from '@backstage/core-plugin-api';
import { AsyncState } from 'react-use/lib/useAsync';
import { ComponentProps } from 'react';
import { JsonObject } from '@backstage/types';
import { PropsWithChildren } from 'react';
import { default as React_2 } from 'react';
import { SearchQuery } from '@backstage/plugin-search-common';
import { SearchResultSet } from '@backstage/plugin-search-common';

// @public (undocumented)
export interface SearchApi {
  // (undocumented)
  query(query: SearchQuery): Promise<SearchResultSet>;
}

// Warning: (ae-forgotten-export) The symbol "QueryResultProps" needs to be exported by the entry point index.d.ts
// Warning: (ae-missing-release-tag) "SearchApiProvider" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public
export function SearchApiProviderForStorybook(
  props: PropsWithChildren<QueryResultProps>,
): JSX.Element;

// @public (undocumented)
export const searchApiRef: ApiRef<SearchApi>;

// @public (undocumented)
export const SearchContextProvider: ({
  initialState,
  children,
}: React_2.PropsWithChildren<{
  initialState?: SearchContextState | undefined;
}>) => JSX.Element;

// Warning: (ae-missing-release-tag) "SearchContextProvider" is exported by the package, but it is missing a release tag (@alpha, @beta, @public, or @internal)
//
// @public
export const SearchContextProviderForStorybook: (
  props: ComponentProps<typeof SearchContextProvider> & QueryResultProps,
) => JSX.Element;

// @public (undocumented)
export type SearchContextState = {
  term: string;
  types: string[];
  filters: JsonObject;
  pageCursor?: string;
};

// Warning: (ae-forgotten-export) The symbol "SearchContextValue" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
export const useSearch: () => SearchContextValue;

// (No @packageDocumentation comment for this package)
```