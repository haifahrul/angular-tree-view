Example:
<app-tree-view
      [data]="listTreeData"
      [selectAll]="selectAll"
      [collapseAll]="collapseAll"
      (onClick)="click($event)"
      (onChange)="onChange($event)">
    <div class="btn-toolbar" role="toolbar" aria-label="Toolbar with button groups">
      <div class="btn-group mr-2" role="group" aria-label="First group">
        <button type="button" class="btn btn-sm btn-secondary" (click)="collapseAll = true">Collapse All</button>
        <button type="button" class="btn btn-sm btn-secondary" (click)="collapseAll = false">Expand All</button>
      </div>
      <div class="btn-group" role="group" aria-label="Second group">
        <button type="button" class="btn btn-sm btn-secondary" (click)="selectAll = true">Check All</button>
        <button type="button" class="btn btn-sm btn-secondary" (click)="selectAll = false">Uncheck All</button>
      </div>
    </div>
