# Angular 2+
1 Don't use button and mat-checkbox together on mat-menu-item.
  - Problem: If you wish keep the menu opened, the $event.stopPropagation() will stop the event to checkbox (It won't change the value on ngModel).
  - Example:  
    `<mat-menu>
      <button mat-menu-item (click)="$event.stopPropagation()">
        <mat-checkbox [(ngModel)]="flag">test</mat-checkbox>        
      </button>
    </mat-menu>
    `
