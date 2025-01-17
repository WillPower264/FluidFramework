## API Report File for "@fluidframework/tinylicious-driver"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { IRequest } from '@fluidframework/core-interfaces';
import { IResolvedUrl } from '@fluidframework/driver-definitions';
import { ITokenProvider } from '@fluidframework/routerlicious-driver';
import { ITokenResponse } from '@fluidframework/routerlicious-driver';
import { IUrlResolver } from '@fluidframework/driver-definitions';
import { ScopeType } from '@fluidframework/protocol-definitions';

// @public (undocumented)
export const createTinyliciousCreateNewRequest: (documentId?: string | undefined) => IRequest;

// @public
export const defaultTinyliciousEndpoint = "http://localhost";

// @public
export const defaultTinyliciousPort = 7070;

// @public
export class InsecureTinyliciousTokenProvider implements ITokenProvider {
    constructor(
    scopes?: ScopeType[] | undefined);
    // (undocumented)
    fetchOrdererToken(tenantId: string, documentId?: string): Promise<ITokenResponse>;
    // (undocumented)
    fetchStorageToken(tenantId: string, documentId: string): Promise<ITokenResponse>;
}

// @public
export class InsecureTinyliciousUrlResolver implements IUrlResolver {
    constructor(port?: number, endpoint?: string);
    // (undocumented)
    getAbsoluteUrl(resolvedUrl: IResolvedUrl, relativeUrl: string): Promise<string>;
    // (undocumented)
    resolve(request: IRequest): Promise<IResolvedUrl>;
}

// (No @packageDocumentation comment for this package)

```
